# VPN Server Configuration Project

This project provides a comprehensive solution for setting up a VPN server with support for various technologies, including OpenVPN, WireGuard, and ShadowSocks. Additionally, Pi-hole is included for content filtering and blocking, along with domain name configuration. A caching DNS server, Unbound, is also deployed to reduce page load times.

The solution is fully configured. The only required step is to update the `.env` file with the following details:
- **For WireGuard:** Specify the host address and the WebGUI password.
- **For ShadowSocks:** Set the server access password.
- **For Pi-hole:** Define the WebGUI password and later upload the necessary blocklist databases.
- **For OpenVPN:** No additional configuration is needed.

## Resources for Configuring WireGuard
- [WireGuard Installation](https://www.wireguard.com/install/) (Download clients and view configuration options)
- [Setting Up WireGuard with a Web Interface](https://telegra.ph/WireGuard-s-veb-interfejsom-05-24) (Guide on setting up WireGuard with WebGUI in Docker)
- [wg-easy GitHub Repository](https://github.com/WeeJeWel/wg-easy#updating)
- [CyberForum Guide](https://www.cyberforum.ru/linux-soft/thread3098886.html) (Instructions on restricting network access for certain users)
- [Keenetic WireGuard Setup Guide](https://help.keenetic.com/hc/ru/articles/360010592379-WireGuard-VPN)
- [Video on Setting Up a Keenetic Router to Connect to a WireGuard Server](https://www.youtube.com/watch?v=fJJJAnyi_tc)

## Resources for Configuring ShadowSocks-libev
- [docker-shadowsocks-libev GitHub Repository](https://github.com/Acris/docker-shadowsocks-libev)
- [Quick Setup Guide for ShadowSocks in Docker](https://itdog.info/podnimaem-shadowsocks-na-servere-po-bystromu/)
- [ShadowSocks Setup Video](https://www.youtube.com/watch?v=udmC5XGaqXk)

## Resources for Configuring OpenVPN
- [OpenVPN-AS GitHub Repository](https://docs.linuxserver.io/deprecated_images/docker-openvpn-as/)
- [OpenVPN-AS Docker Setup Guide](https://www.smarthomebeginner.com/install-openvpn-access-server-using-docker/)
- [OpenVPN Video Guide](https://www.youtube.com/watch?v=mVwT4FzvvKc) (Comprehensive video guide on OpenVPN)
- [Video on Setting Up an OpenVPN Tunnel Between Offices](https://www.youtube.com/watch?v=S358miThwdg)
- [OpenVPN on Mikrotik Setup Video](https://www.youtube.com/watch?v=3dEYm9c71Nc)

## Resources for Configuring Pi-hole
- [Guide for Integrating Pi-hole with WireGuard](https://www.juev.org/2020/05/01/wireguard-pi-hole/)
- [Pi-hole Docker GitHub Repository](https://github.com/pi-hole/docker-pi-hole#readme)
- [Firebog - Blocklist Collection](https://firebog.net/)
- [Pi-hole Blocklist Generator](https://sefinek.net/blocklist-generator/pihole)

## Setting Up Docker on a New Host
- [Docker Installation Guide for Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
- [Docker Post-Installation Steps](https://docs.docker.com/engine/install/linux-postinstall/) (Including permission settings)

## SSH Configuration
- [SSH Setup Guide for Ubuntu](https://selectel.ru/blog/ssh-ubuntu-setup/)

## Fail2Ban Configuration
- [Fail2Ban Setup Guide](https://www.dmosk.ru/instruktions.php?object=fail2ban) (For configuring Fail2Ban on a new server)


# Проект по настройке VPN сервера

Данный проект представляет собой комплексное решение для организации VPN сервера с поддержкой различных технологий, таких как OpenVPN, WireGuard и ShadowSocks. Также добавлен Pi-hole для фильтрации и блокировки ненужного контента и настройки доменных имен. В дополнение к нему развернут кэширующий DNS-сервер Unbound для сокращения времени загрузки страниц.

Решение полностью настроено, из необходимого нужно лишь внести изменения в файл `.env`:
- **Для WireGuard:** Укажите адрес хоста и пароль для WebGUI.
- **Для ShadowSocks:** Установите пароль для доступа к серверу.
- **Для Pi-hole:** Задайте пароль для WebGUI и впоследствии загрузите необходимые базы для блокировок.
- **Для OpenVPN:** Дополнительная настройка не требуется.

## Ресурсы для настройки WireGuard
- [Установка WireGuard](https://www.wireguard.com/install/) (Здесь можно скачать клиенты и посмотреть варианты конфигурации)
- [Настройка WireGuard с веб-интерфейсом](https://telegra.ph/WireGuard-s-veb-interfejsom-05-24) (Руководство по настройке WireGuard с WebGUI в Docker)
- [Репозиторий wg-easy на GitHub](https://github.com/WeeJeWel/wg-easy#updating)
- [Руководство на CyberForum](https://www.cyberforum.ru/linux-soft/thread3098886.html) (Инструкция по запрету доступа к остальной сети для некоторых пользователей)
- [Статья Keenetic по настройке WireGuard](https://help.keenetic.com/hc/ru/articles/360010592379-WireGuard-VPN)
- [Видео по настройке роутера Keenetic для подключения к серверу WireGuard](https://www.youtube.com/watch?v=fJJJAnyi_tc)

## Ресурсы для настройки ShadowSocks-libev
- [Репозиторий docker-shadowsocks-libev на GitHub](https://github.com/Acris/docker-shadowsocks-libev)
- [Статья по быстрому запуску ShadowSocks в Docker](https://itdog.info/podnimaem-shadowsocks-na-servere-po-bystromu/)
- [Видео по настройке подключения ShadowSocks](https://www.youtube.com/watch?v=udmC5XGaqXk)

## Ресурсы для настройки OpenVPN
- [Репозиторий OpenVPN-AS на GitHub](https://docs.linuxserver.io/deprecated_images/docker-openvpn-as/)
- [Руководство по настройке OpenVPN-AS в Docker](https://www.smarthomebeginner.com/install-openvpn-access-server-using-docker/)
- [Видео-гайд по OpenVPN](https://www.youtube.com/watch?v=mVwT4FzvvKc) (Подробный видео-гайд по OpenVPN)
- [Видео о настройке туннеля OpenVPN между офисами](https://www.youtube.com/watch?v=S358miThwdg)
- [Видео по настройке OpenVPN на Mikrotik](https://www.youtube.com/watch?v=3dEYm9c71Nc)

## Ресурсы для настройки Pi-hole
- [Руководство по интеграции Pi-hole и WireGuard](https://www.juev.org/2020/05/01/wireguard-pi-hole/)
- [Репозиторий Pi-hole на Docker](https://github.com/pi-hole/docker-pi-hole#readme)
- [Firebog - коллекция баз для блокировок](https://firebog.net/)
- [Конструктор баз для блокировок Pi-hole](https://sefinek.net/blocklist-generator/pihole)

## Настройка Docker на новом хосте
- [Руководство по установке Docker на Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
- [Постинсталляционные шаги для Docker](https://docs.docker.com/engine/install/linux-postinstall/) (Включая настройку прав доступа)

## Настройка SSH
- [Руководство по настройке SSH на Ubuntu](https://selectel.ru/blog/ssh-ubuntu-setup/)

## Настройка Fail2Ban
- [Руководство по настройке Fail2Ban](https://www.dmosk.ru/instruktions.php?object=fail2ban) (Для настройки Fail2Ban на новом сервере)
