---
description: Docker Hub Automated Builds
keywords: Docker, webhookds, хаб, сборки
title: Веб-хаки для автоматизированных сборок
---

Если в Docker Hub имеется автоматизированный репозиторий сборки, вы можете использовать Webhooks, чтобы вызвать действие в другом приложении в ответ на событие в репозитории. Webhook - это запрос POST, отправленный на определенный URL-адрес, который предоставляет услугу. Docker Hub webhooks загорается, когда изображение встроено или добавлен новый тег, в ваш автоматизированный репозиторий сборки.

Настройте веб-узлы на `https://hub.docker.com/r/<USERNAME>/<REPOSITORY>/~/settings/webhooks/`.

![Create Webhook](/docker-hub/images/webhooks.png)

С вашим веб-узлом вы указываете целевой URL-адрес для POST. Docker Hub POST отправляет URL-адрес со следующей полезной нагрузкой:

```json
{
  "callback_url": "https://registry.hub.docker.com/u/svendowideit/testhook/hook/2141b5bi5i5b02bec211i4eeih0242eg11000a/",
  "push_data": {
    "images": [
        "27d47432a69bca5f2700e4dff7de0388ed65f9d3fb1ec645e2bc24c223dc1cc3",
        "51a9c7c1f8bb2fa19bcd09789a34e63f35abb80044bc10196e304f6634cc582c",
        "..."
    ],
    "pushed_at": 1.417566161e+09,
    "pusher": "trustedbuilder",
    "tag": "latest"
  },
  "repository": {
    "comment_count": "0",
    "date_created": 1.417494799e+09,
    "description": "",
    "dockerfile": "#\n# BUILD\u0009\u0009docker build -t svendowideit/apt-cacher .\n# RUN\u0009\u0009docker run -d -p 3142:3142 -name apt-cacher-run apt-cacher\n#\n# and then you can run containers with:\n# \u0009\u0009docker run -t -i -rm -e http_proxy http://192.168.1.2:3142/ debian bash\n#\nFROM\u0009\u0009ubuntu\n\n\nVOLUME\u0009\u0009[\/var/cache/apt-cacher-ng\]\nRUN\u0009\u0009apt-get update ; apt-get install -yq apt-cacher-ng\n\nEXPOSE \u0009\u00093142\nCMD\u0009\u0009chmod 777 /var/cache/apt-cacher-ng ; /etc/init.d/apt-cacher-ng start ; tail -f /var/log/apt-cacher-ng/*\n",
    "full_description": "Автоматизированная сборка Docker Hub с репо GitHub",
    "is_official": false,
    "is_private": true,
    "is_trusted": true,
    "name": "testhook",
    "namespace": "svendowideit",
    "owner": "svendowideit",
    "repo_name": "svendowideit/testhook",
    "repo_url": "https://registry.hub.docker.com/u/svendowideit/testhook/",
    "star_count": 0,
    "status": "Active"
  }
}
```

>**Примечание**:  Если вы хотите протестировать свой webhook, мы рекомендуем использовать инструмент, например requestb.in . Также обратите внимание, что сервер Docker Hub нельзя фильтровать по IP-адресу.
