## Эталонная структура и что-то там

1. Сеть пользователя (User Network / customer premises network)
2. Сеть доступа (Access network) (Radio Access Network)
    - RAT (Radio access technologies) (для радио)
    - ANT (для проводных)
3. Ядро сети (Core Network)
4. Сеть услуг (Service network)

User net. $\xLeftrightarrow{Lastmile}$ Access net. $\xLeftrightarrow{Backhaul}$ Core net. $\xLeftrightarrow{Backbone}$ Service net.

### Распределительная сеть (distribution system)
- Уровень доступа
- Уровень агрегации
- уровень ядра

### Схема итмо (UPD: нет)

Точки доступа $\implies$ Контроллеры $\implies$ Коммутатор $\implies$ Шлюз (Маршрутизатор, фильтр трафика) $\implies$ Интернет

К коммутаторам также входит система управления (NMS) и система безопасности (AAA).

**Сеть доступа**:
- Элементы:
    - Точки доступа
    - Контрллеры

**Ядро сети**:
- Элементы:
    - Коммутаторы
    - Шлюз
- RAT:
    - WiFi 2.4(802.11/b/g/n)
    - WiFi 2.4(802.11/a/n)

**Сеть услуг**:
- Элементы
    - Интернет
    - Runnet?
- CNT:
    - Fast ethernet
    - Gigabit
    - 10GIgabit

Уровень доступа:
- Элементы:
    - Точки доступа
    - Контролллеры
Уровень агрегации
- Элементы:
    - Комутатор
Уровень ядра
- Элементы
    - Шлюз
    - Интернет

Поехали примеры:
- Что-то (ТВ, ПК)
- Что-то еще (Беспроводной маршрутизатор, GPON, STB)

А это что? Еще одна схема?
БС $\iff$ Контроллер* $\iff$ SGSN $\iff$ GGSN $\iff$ Интернет
БС $\iff$ Контроллер* $\iff$ SMSC $\iff$ GMSC $\iff$ TPON

SMSC - мобильный центр коммутации
PDN - package data network
TPON - телефонная что-то общего пользования

#### AAA (это не ор, а название чего-то)
Au $\iff$ EIR $\iff$ HLR $\iff$ VLR
EIR - ??
HLR - регистер местоположения домашних абонентов
VLR - местоположение гостевых абонентов
#### NMS
OAM - система технологической поддержки и эксплуатации сети

### Еще какая-то подтема
ТХ - Среда передачи - RX
TX:
- Передатчик (КИ, КК, М)
- Вспомагательные системы
- Система электропитания
RX:
- Приемник (ДКИ, ДКК, ДМ)
- СЭ
- Вспомагательная система
*Д - значит де что-то. А что такое КИ/КК/М вопрос другой
М - модулятор
КК - кодек канала
КИ - кодек Источника
ИС $\iff$ КИ $\iff$ КК $\iff$ М $\iff$ Среда передачи $\iff$ ДМ $\iff$ ДКК $\iff$ ДКИ $\iff$ ПС