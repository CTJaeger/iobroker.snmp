# Информация об адаптере SNMP

## Главная Информация

Протокол SNMP (Simple Network Management Protocol) был разработан для централизованного управления всеми сетевыми устройствами. К ним относятся принтеры, маршрутизаторы, коммутаторы, серверы, компьютеры и т. Д.

Адаптер SNMP использует так называемый OID (идентификатор объекта) для считывания этих значений с соответствующего устройства.

## Администрирование / Страница администратора
! [Adapter_admin_konfiguration] (IMG/adminpage.png)

1. RetryTimeout - время повтора в мс
2. connectTimeout - попытка подключения в мс
3. pollInterval - период опроса каждые XXXX мс

## Принтеры

Для большинства принтеров есть стандарт. (PRINTER MIB)
http://www.oidview.com/mibs/0/Printer-MIB.html

Для цветного лазера Samsung CLP320, например. следующие идентификаторы OID действительны.

Количество печатных страниц: 1.3.6.1.2.1.43.10.2.1.4.1.1

Черный тонер: 1.3.6.1.2.1.43.11.1.1.9.1.1

Тонер голубой: 1.3.6.1.2.1.43.11.1.1.9.1.2

Тонер пурпурный: 1.3.6.1.2.1.43.11.1.1.9.1.3

Тонер желтый: 1.3.6.1.2.1.43.11.1.1.9.1.4

Блок Life_drum: 1.3.6.1.2.1.43.11.1.1.9.1.7

## NAS Systems - пример

Synology: по умолчанию SNMP отключен на Synology Diskstations и должен быть включен в WebUI. Важно, чтобы порт 161 по умолчанию оставался и сообщество настроено правильно. В основном это публично.

https://global.download.synology.com/download/Document/MIBGuide/Synology_DiskStation_MIB_Guide.pdf

## Поиск производителя и MIB в большинстве случаев является успешным.
