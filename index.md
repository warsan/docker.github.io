---
description: Домашняя страница документации Docker
keywords: Docker, documentation, manual, guide, reference, api, samples
landing: true
title: Документация докеров
notoc: true
notags: true
---
{% assign page.title = site.name %}

<div class="row">
<div markdown="1" class="col-xs-12 col-sm-12 col-md-12 col-lg-6 block">

## Начать с Docker

Прочтите наше новое многоэтапное пошаговое руководство, описывающее создание первого приложения, 
хранения данных, сетей и роев и заканчивается тем, что приложение работает 
на сервере в облаке. Общее время чтения меньше часа.

[Get started with Docker](/get-started/){: class="button outline-btn"}

</div>
<div markdown="1" class="col-xs-12 col-sm-12 col-md-12 col-lg-6 block">

## Пробуйте Docker Enterprise Edition

Запустите свое решение с помощью Docker Enterprise Edition, чтобы получить панель управления, сканирование безопасности, интеграцию с LDAP, подписание контента, поддержку нескольких облаков и многое другое. 
Нажмите ниже, чтобы протестировать запущенный экземпляр Docker, не устанавливая ничего.

[Попробуйте Docker Enterprise Edition](https://dockertrial.com){: class="button outline-btn" onclick="ga('send', 'event', 'EE Trial Referral', 'Front Page', 'Click');"}

</div>
</div>

## Докеры

<div class="row">
<div markdown="1" class="col-xs-12 col-sm-12 col-md-12 col-lg-6 block">

### Сообщество разработчиков Docker

Начните работу с Docker и экспериментируйте с приложениями на основе контейнеров. Docker CE 
доступен на многих платформах: от настольных до облачных до серверов. 
Можно строить, делиться контейнерами и автоматизировать конвейер разработки из одной среды. 
Выберите канал «Край», чтобы получить доступ к последним функциям, или «Стабильный» 
канал для большей предсказуемости.

[Узнайте больше о Docker CE](/install/index.md#platform-support-matrix){: class="button outline-btn"}

</div>
<div markdown="1" class="col-xs-12 col-sm-12 col-md-12 col-lg-6 block">

### Docker Enterprise Edition

Предназначен для разработчиков и ИТ-специалистов, которые строят, отправляют и запускают 
критически важные для бизнеса приложения в масштабе производства. Интегрированные, сертифицированные, 
и поддерживаемые для обеспечения предприятий самой безопасной контейнерной платформой в 
промышленности для модернизации всех приложений. Docker EE Advanced поставляется с корпоративными
[add-ons](#docker-ee-add-ons) как UCP и DTR.

[Learn more about Docker EE](/install/#platform-support-matrix){: class="button outline-btn"}

</div>
</div><!-- конечная строка -->

## Запустить Docker где угодно

<div class="component-container">
    <!--start row-->
    <div class="row">
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="docker-for-mac/"> <img src="../images/apple_48.svg" alt="Docker для Mac"> </a>
                </div>
                <h3 id="docker-for-mac"><a href="docker-for-mac/">Docker для Mac</a></h3>
                <p>Натуральное приложение с использованием песочницы для MacOS, предоставляет все инструменты Docker для вашего Mac.</p>
            </div>
        </div>
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="docker-for-windows/"> <img src="../images/windows_48.svg" alt="Docker для Windows"> </a>
                </div>
                <h3 id="docker-for-windows"><a href="docker-for-windows/">Docker для Windows</a></h3>
                <p>Приложение Windows предоставляет все инструменты Docker на вашем компьютере.</p>
            </div>
        </div>
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="install/linux/ubuntu/"> <img src="../images/linux_48.svg" alt="Docker для Linux"> </a>
                </div>
                <h3 id="docker-for-linux"><a href="install/linux/ubuntu/">Docker для Linux</a></h3>
                <p>Docker для компьютера, на котором установлен дистрибутив Linux.</p>
            </div>
        </div>
    </div>
</div>

<div class="component-container">
    <!--start row-->
    <div class="row">
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="docker-cloud/"> <img src="../images/cloud_48.svg" alt="Docker Cloud"> </a>
                </div>
                <h3 id="docker-cloud"><a href="docker-cloud/">Docker Cloud</a></h3>
                <p>Хостинг-служба для создания, тестирования и развертывания Docker для ваших хостов.</p>
            </div>
        </div>
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="docker-for-aws/"> <img src="../images/cloud_48.svg" alt="Docker для AWS"> </a>
                </div>
                <h3 id="docker-cloud-providers"><a href="docker-for-aws/">Docker для AWS</a></h3>
                <p>Разверните Docker на AWS.</p>
            </div>
        </div>
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="docker-for-azure/"> <img src="../images/cloud_48.svg" alt="Docker для Azure"> </a>
                </div>
                <h3 id="docker-cloud-providers"><a href="docker-for-azure/">Docker для Azure</a></h3>
                <p>Разверните Docker на Azure.</p>
            </div>
        </div>
    </div>
</div>

## Компоненты

<h5>Docker EE Add-ons</h5>

<div class="component-container">
    <!--start row-->
    <div class="row">
    <!--UCP-->
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="datacenter/ucp/{{ site.ucp_version }}/guides/"> <img src="../images/UCP_48.svg" alt="Универсальный пульт"> </a>
                </div>
                <h3 id="ucp"><a href="datacenter/ucp/{{ site.ucp_version }}/guides/">Универсальный пульт</a></h3>
                <p>(UCP) Управляйте кластером локальных хостов Docker как отдельной машиной с этим корпоративным продуктом.</p>
            </div>
        </div>
    <!--DTR-->
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="datacenter/dtr/{{ site.dtr_version }}/guides/"> <img src="../images/dtr_48.svg" alt="Docker Trusted Registry"> </a>
                </div>
                <h3 id="dtr"><a href="datacenter/dtr/{{ site.dtr_version }}/guides/">Docker Trusted Registry</a></h3>
                <p>(DTR) An enterprise image storage solution you can install behind a firewall to manage images and access.</p>
            </div>
        </div>
    </div>
    <!-- end real row-->
</div>

<h5>Docker Tools</h5>

<div class="component-container">
    <!--start row-->
    <div class="row">
    <!--compose-->
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="compose/overview/"> <img src="../images/compose_48.svg" alt="Docker Compose"> </a>
                </div>
                <h3 id="compose"><a href="compose/overview/">Docker Compose</a></h3>
                <p>Define application stacks built using multiple containers, services, and swarm configurations.</p>
            </div>
        </div>
    <!--machine-->
        <div class="col-sm-12 col-md-12 col-lg-4 block">
            <div class="component">
                <div class="component-icon">
                    <a href="machine/overview/"> <img src="../images/machine_48.svg" alt="Docker Trusted Registry"> </a>
                </div>
                <h3 id="machine"><a href="machine/overview/">Docker Machine</a></h3>
                <p>Automate container provisioning on your network or in the cloud. Available for Windows, macOS, or Linux.</p>
        </div>
    </div>
</div>


<!-- end component-container 2-->
</div>
