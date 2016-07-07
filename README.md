
![DayLight](http://i.imgur.com/bCNkzd4.png)

**DayLight** - концепция финансовой и государственной системы, построенных на базе блокчейна.

ЦБ одной страны не должен доверять ЦБ другой страны. Для того, чтобы осуществить транзакцию обмена одной валюты на другую нам необходимо знать баланс, а как следствие историю всех операций по данному счету. Поэтому у каждого ЦБ должна быть информация обо всех счетах во всех валютах. В этом случае не только ЦБ, но и весь рынок будет знать объем эмиссированных другими ЦБ средств.

Т.к. ЦБ разных стран не могут полагаться на какой-то один центральный орган, единственным вариантом будет использование блокчейна для обмена данными.

ЦБ должен быть уверен в том, что баланс счета в неподконтрольной ему валюте именно такой, какой заявлено. Для этого ему необходимо пропускать через свою ноду все транзакции, связанные с этим счетом. А именно: пополнение и списание средств со счета при помощи  переводов от других граждан, компаний (покупки, продажи, зарплаты, дивиденды, распределение прибыли), государства (налоги, зарплаты), ЦБ (эмиссия).

**DayLight отличается от существующей финансовой и государственной системы открытостью и отсутствием ненужных посредников.**


![DayLight schema](http://i.imgur.com/eI64rzv.png)


Часть транзакций в будущем (я надеюсь в ближайшие годы) должны будут генерироваться искусственным интеллектом, когда он на это будет способен. А пока что они будет создаваться людьми. Лично для меня, DayLight - это платформа, которая сделает переход классической системы управления государством к системе, где вместо чиновников большинство решений принимает ИИ. В будущем, которое я хочу сделать политики и чиновники - это высокообразованные айтишники, способные анализировать предлагаемые ИИ решения.

**DayLight может существовать параллельно с классической финансовой и государственной системой, постепенно производя их замену**

-------

ЦБ

* [ЦБ](#ЦБ)
* [Смена IP ноды ЦБ](#Смена-ip-ноды-ЦБ)
* [Эмиссия-валюты](#Эмиссия-валюты)
* [Выбор главы ЦБ](#Выбор-главы-ЦБ)
* [Кредитование](#Кредитование)
* [Регистрация представителя ЦБ](#Регистрация-представителя-ЦБ)
* [Отзыв лицензии у представителя ЦБ](#Отзыв-лицензии-у-представителя-ЦБ)
* [Установка параметров по анонимным счетам](#Установка-параметров-по-анонимным-счетам)

Граждане

* [Перевод средств](#Перевод-средств)
* [p2p кредитование](#p2p-кредитование)
* [Запрос на продажу недвижимости](#Запрос-на-продажу-недвижимости)
* [Запрос на кредит](#Запрос-на-кредит)
* [Регистрация брака](#Регистрация-брака)
* [Расторжение брака](#Расторжение-брака)
* [Брачный контракт](#Брачный-контракт)
* [Покупка товаров на аукционе](#Покупка-товаров-на-аукционе)
* [Оформление наследства](#Оформление-наследства)
* [Создание партии](#Создание партии)
* [Выбор главы гос-ва](#Выбор-главы-гос-ва)
* [Голование за партию](#Голование-за-партию)
* [Выборы сенаторов](#Выборы-сенаторов)

Государство

* [Настройка параметров государства](#Настройка-параметров-государства)
* [Срок полномочий губернаторов](#Срок-полномочий-губернаторов)
* [Выборы губернатора](#Выборы-губернатора)
* [Назначение органов местной власти](#Назначение-органов-местной-власти)
* [Регистрация гражданина](#Регистрация-гражданина)
* [Налогообложение](#Налогообложение)
* [Добавление объекта недвижимости](#Добавление-объекта-недвижимости)
* [Загрузка федерального бюджета](#Загрузка-федерального-бюджета)

Компании

* [Регистрация компании](#Регистрация-компании)
* [Расходные проводки](#Расходные-проводки)
* [Регистрация товаров](#Регистрация-товаров)
* [Регистрация Item компанией](#Регистрация-Item-компанией)
* [Периодичность выплаты зарплаты в компании](#Периодичность-выплаты-зарплаты-в-компании)
* [Прием гражданина на работу](#Прием-гражданина-на-работу)
* [Увольнение сотрудника](#Увольнение-сотрудника)
* [Начисление премии сотруднику](#Начисление-премии-сотруднику)
* [Регистрация доверенного лица ген. директора](#Регистрация-доверенного-лица-ген.-директора)
* [Покупка товара компанией у компании](#Покупка-товара-компанией-у-компании)
* [Списание товара с баланса компании](#Списание-товара-с-баланса-компании)
* [Выписка счета](#Выписка-счета)
* [Выпуск акции](#Выпуск-акции)
* [Ликвидация компании](#Ликвидация-компании)
* [Buy/Sell акций](#buysell-акций)
* [Обмен валюты](#Обмен-валюты)
* [Краудфандинг](#Краудфандинг)

---

### ЦБ

###### CentralBanks
| ID        | CurrencyId           | NodeIp  | UserId  |
| ------------- |-------------| -----|-----|

Все 159 ЦБ зарегистрированы заранее в таблице CentralBanks. 


### Смена IP ноды ЦБ
```
TX
 * NodeIp
 * UserId
 * Подпись главы ЦБ
```

###### ChangeCBNodeIpHistory
| ID        | CBID | UserId           | NodeIp  | BlockId  |
| ------------- |-------------| -----|-----|-----|


### Эмиссия валюты

Начисление средств на счета всех граждан
```
TX1
 * ID валюты
 * Сумма
 * Подпись главы ЦБ
```
###### EmissionHistoryAmount
| ID        | CurrencyId           | Amount  | BlockId  |
| ------------- |-------------| -----| -----|
Увеличение средств на определенный процент
```
TX2
 * ID валюты
 * Процент
 * Подпись главы ЦБ
```
###### EmissionHistoryPct
| ID        | CurrencyId           |  Pct  | BlockId  |
| ------------- |-------------| -----| -----|-----|

Увеличение средств на кредитных счетах
```
TX2
 * ID валюты
 * Сумма
 * Процент
 * Подпись главы ЦБ
```
###### EmissionHistoryCredit
| ID        | CurrencyId           |  Amount  | Pct  | BlockId  |
| ------------- |-------------| -----|-----|-----|-----|

Вместо выкупа гос. облигаций ЦБ будут осуществлять эмиссию при помощи прямого зачисления средств на счета своих граждан. Если эмиссия не должна повлечь перманентное увеличение денежной массы, тогда ЦБ может начислить средства на кредитные счета граждан.

Операции добавления средств миллиарду граждан будут очень ресурсозатратными, поэтому их нужно делать в несколко итараций в течение нескольких часов.

### Выбор главы ЦБ

```
TX
 * ID валюты
 * ID голосующего гражданина
 * ID гражданина, который будет выбран главой ЦБ
 * Подпись голосующего гражданина
```

###### VoteCBHistory
| ID        | UserId           | VoteUserId  | Time  | BlockId  |
| ------------- |-------------| -----|-----|-----|

Держатели валюты раз в X дней выбирают главу ЦБ, той стран, в которой они зарегистрированы.

### Создание партии

```
TX
 * Название партии
 * Описание
 * Подпись гражданина
```

Если в настройках параметров государства выбрана мультипартийная политическая система, тогда любой гражданин достигший определнного в парметрах возраста может создать свою партию.

###### PoliticalParties
| ID        | Name           | Description  | Time  | 
| ------------- |-------------| -----|-----|

### Голосование за партию

```
TX
 * ID партии
 * ID голосующего гражданина
 * Подпись голосующего гражданина
 ```

###### VotePoliticalPartiesHistory
| ID        | UserId           | PoliticalPartyId  | Time  | BlockId  |
| ------------- |-------------| -----|-----|-----|

### Выборы сенаторов

```
TX
 * ID гржданина
 * ID голосующего гражданина
 * Подпись голосующего гражданина
 ```

###### VoteSenatorsHistory
| ID        | UserId           | VoteUserId  | Time  | BlockId  |
| ------------- |-------------| -----|-----|-----|



### Выбор главы гос-ва

```
TX
 * ID гражданина, который будет выбран главой гос-ва
 * ID голосующего гражданина
 * Подпись голосующего гражданина
 ```

###### VoteHeadOfStateHistory
| ID        | UserId           | VoteUserId  | Time  | BlockId  |
| ------------- |-------------| -----|-----|-----|

Глава государства имеет право устанавливать размер налогов, загружать в блокчейн бюджет страны. Но при изменении настроек парметров гос-ва разлиные функции могут быть переданы дрпугим органам власти.


### Настройка параметров государства
```
TX
 * Настройки (JSON)
 * UserId главы гос-ва
 * Подпись главы гос-ва
 ```

###### CountryOptions
| CountryId        | Options           | PresidentUserId  |
| ------------- |-------------| -----|


Каждая страна может настроить свою политическую систему. Кол-во партий, их полномочия, полномочия главы гос-ва и т.д.

### Срок полномочий губернаторов
```
TX
 * Кол-во лет
 * Подпись главы гос-ва
 ```


### Выборы губернатора

```
TX
 * ID гражданина, который будет выбран губернатором
 * ID голосующего гражданина 
 * Подпись голосующего гражданина
 ```
Гражданин может голосовать за губернатора, зарегистрированного в том же городе, где и он сам.

###### VoteGovernorHistory
| ID        | UserId           | VoteUserId  | Time  | BlockId  |
| ------------- |-------------| -----|-----|-----|


### Назначение органов местной власти

```
TX
 * ID гражданина, который будет выбран в орган местной власти
 * Подпись голосующего гражданина
 ```

###### VoteLocalAuthoritiesHistory
| ID        | UserId           | VoteUserId  | Time  | BlockId  |
| ------------- |-------------| -----|-----|-----|


### Регистрация гражданина

```
TX
 * Личные данные (private)
 * Страна
 * Штат
 * Город
 * Дата рождения
 * Public key
 * User ID органа местной власти
 * Подпись органа местной власти
 ```

###### Users

| ID        | Личные данные (private)           | Страна | Штат | Город | Дата рождения | Public key  | GovUserId  | Status  | BlockId  |
| ------------- | ------------- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- |

Дата рождения, и местонаждение необходимы для участие в выборах в органы власти.

###### UsersAccounts
Пользователю автоматически создается счет в той валюте, которой управляет ЦБ

| ID        | CurrencyId           | UserId  | Amount  |
| ------------- |-------------| -----|-----|
Если UserId = 0, значит счет анонимный и к нему применяются особые лимиты, устанавливаемые главой ЦБ.
Новых пользователей могут регистрировать только представители ЦБ

### Фиксирование смерти гражданина

```
TX
 * User ID
 * User ID органа местной власти
 * Подпись органа местной власти
 ```
 
В результате этой транзакции в таблице Users status ставновится равен "умер", в резльтате чего становится возможным выполнение смарт-контракта, распределяющего наследство. Если такого смарт-контракта нет, тогда все средства и имущество умершего гражданина автоматически распределяется между его самыми близкими родставенниками.

###### UsersDiedHistory
| ID        | UserId           | Time  | GovUserId  | BlockId  |
| ------------- |-------------| -----| -----| -----|

### Кредитование


 
#### Перевод средств с кредитного счета на расчетный
 
```
TX
 * Сумма, которая будет перечислена с UsersCBLoans на расчетный счет UsersAccounts
 * UsersCBLoans ID
 * Подпись пользователя
 ```
 
###### UsersCBLoans

| ID        | CurrencyId           | UserId  | Amount  | Pct  | BlockId  |
| ------------- |-------------| -----|-----|-----|-----|

ЦБ может начислить всем гражданам своей страны какую-то сумму, которую гражданин может израсходовать всю или частично. Например, ЦБ США начислил всем по $10 000 кредитных средств под 0,25%/год. Если Вам нужно $3000, то можно взять только их из $10 000 и платить % нужно будет именно с $3000. Под словом "взять" я имею виду, что нужно будет перевести их на свой обычный расчетный счет (UsersAccounts). 

#### Платеж по кредиту

```
TX
 * Платеж по кредиту
 * UsersLoans ID
 * Подпись пользователя
 ```
 
###### UsersLoans
| ID        | CurrencyId           | Amount  | Pct | Remain  | PledgeItemId | MonthPayment | LastPayment  | CreateTime  | DefaultPeriod |
| ------------- |-------------| -----|-----|------------- |-------------| -----|-----|-----|-----|
После того, как кредитные средства попадают на расчетный счет (UsersAccounts) создается запись в UsersLoans, где отмечается размер кредита, который гражданин должен вернуть. Если это массовый кредит от ЦБ, то Pledge будет пустое. В момент создания записи Amount=Remain. После каждой выплаты по кредиту, Remain пересчитывается. При пересчете учитывается Pct и время предыдущего пересчета Remain, чтоб можно было учесть набежавшие %.
Если кредит под залог, то при отсутствии платежей в размере MonthPayment в течение DefaultPeriod происходит выставление на аукцион залога PledgeItemId (за исключение случаев, когда PledgeItemId является дом или квартира). 


###### UsersLoansHistory
| ID        | UsersLoansId | BlockId |
| ------------- |-------------| -----|

### p2p кредитование

Предложение кредита
```
TX
 * User ID заемщика
 * User ID кредитора
 * Подпись кредитора
```

###### CreditHistoryOffers

| ID        | CurrencyId           | Amount  | Pct | MonthPayment | Creditor | Time | BlockId |
| ------------- |-------------| -----|-----|-----|-----|-----|-----|

Пользователь может одолжить свои средства другому пользователю.

Принятие условий кредита

```
TX
 * CreditHistoryOffers ID
 * User ID заемщика
 * Подпись заемщика
```

Если эта тр-ия была отправлена в течение суток с момента поступления предложения, тогда происходить добавление записи в UsersLoans и начисление средств в UsersAccounts.


### Регистрация представителя ЦБ

```
TX
 * UserId представителя
 * UserId главы ЦБ
 * Подпись главы ЦБ
 ```

###### RepresentativesLicense

| ID        | UserId представителя          | Currency ID  | Status | 
| ------------- |-------------| ----- | ----- | 

Представитель ЦБ может регистрировать счета гражданам, а также одобрять или отклонять запросы на кредиты. Доход представители получают в том случае, если кредит возвращается, если нет - то штраф. Если представитель не хочет обанкротиться, то ему придется одобрять кредит, чтобы получать доход, в то же время, одобряя все кредит он легко может уйти в минус. 


###### RepresentativesLicenseHistory
| ID | RepresentativesLicenseID        |  Status | BlockId | 
| ------------- |-------------|-------------|-------------|


### Отзыв лицензии у представителя ЦБ

```
TX
 * UserId представителя
 * UserId главы ЦБ
 * Подпись главы ЦБ
 ```
 
### Установка параметров по анонимным счетам

```
TX
 * Максимальная сумма поступлений на счет за месяц.
 * Максимальное кол-во людей, от которых могут приходить поступления
 * Подпись представителя ЦБ
```

Анонимные счета нужны гражданам для того, чтобы они могли оплачивать какие-то товары анонимно. В то же время эти счета не должны использовать криминальные структуры для получения нелегальных доходов.

###### AnonymousSettings
| ID        | CurrencyId           | MaxAmount  | MaxPeople  |
| ------------- |-------------| -----|-----|

 
### Регистрация компании
```
TX
 * Название компании
 * Страна
 * Город
 * UserID основателя
 * Подпись основателя
```

###### Companies
| ID        | Name           | Owners (JSON)    | RulesId |
| ------------- | ------------- | ----- | ----- |


На нашей планете есть огромное кол-во вариантов по которым функционируют компании. Все эти варианты должны быть доступны любому гражданину в любой стране. Программный код правила будет описан в DayLight. Для гражданина выбор правил будет в виде каталога, где он может изучить, как именно будет функционировать компания и выбрать желаемый вариант.


###### CompaniesHistory
| ID        | CompanyID        | Name           | Owners (JSON)    | RulesId | BlockId |
| ------------- | ------------- | ----- | ----- |----- |----- |


###### CompaniesAccounts
| ID        | CurrencyId           | CompanyId    | Amount    |
| ------------- |-------------| -----| -----|

### Перевод средств

```
TX
 * SenderType (User|Company)
 * RecipientType (User|Company)
 * Sender UserId
 * Purpose (private for users and public for companies)
 * Recipient UserId
 * Подпись отправителя
```

Человек может отправить средства компании (назначение платежа шифруется), другому человеку (назначение платежа шифруется). Компания может отправить средства другой компании (назначение платежа не шифруется) или человеку (назначение платежа не шифруется).

### Налогообложение

Глава гос-ва (или другой орган, в зависимости от настроек в таблице CountryOptions) устанавливает размер федеральных и региональных налогов. Также он устанавливает, какая часть налога остается в бюджете региона, а какая отправляется в федеральный бюджет.


```
TX
 * Type
 * MinAmount
 * Pct
 * Utensils
 * FedPct
 * Period
 * Подпись главы гос-ва
```

###### Taxes
| ID        | Period           | Type    |Amount    |Pct    |Utensils    |FedPct    |
| ------------- |-------------| -----| -----| -----| -----| -----|

###### TaxesHistory
| ID        | TaxesID | Period           | Type    |Amount    |Pct    |Utensils    |FedPct    | BlockId|
| ------------- |-------------| -----| -----| -----| -----| -----|-----|-----|

Налоги с компаний автоматически снимаются раз в квартал. При списании налога учитывается его тип и минимальная сумма для данного процента, федеральный налог или региональный. Глава правительства может установить минимальную сумму дохода гражданина, с которой подоходный налог не взимается. Аналогично и для компаний - может быть мин. сумма, когда компания освобождается от налогов.

```
TXh
 * TaxesID
 * Вспомогательная подпись главы гос-ва
```
###### TaxesDaemonHistory
| ID        | TaxesID    | BlockId|
| ------------- |-------------| -----|

Вспомогательная тр-ия отправляется автоматически и запускает процесс списания налогов, согласно указанному в таблице Taxes периоду

### Добавление объекта недвижимости
Добавлять объект имеют права органы местной власти.

```
TX
 * Координаты объекта
 * Price
 * Тип объекта
 * Подпись органа местной власти
```

Вы идете по улице, видите заброшенный участок, который владельцу явно не нужен, но Вам он нравится и Вы не против его купить в кредит. Вы отправляете тр-ию с предложением продать участок. Представитель банка автоматически отправляет тр-ию подтверждения кредита (автоматически т.к. алгоритм проанализировал Ваши доходы, начальную стоимость участка и решил, что кредит с вероятностью 99,9% будет погашен). Владелец участка получает уведомление, что есть запрос на покупку. Если цена устраивает владельца участка, то ему нужно будет нажать кнопку "продать".


###### Property
| ID        | Coords  | Price  | CityId  | Owner type (user or company) | Owners (JSON) | BlockId |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |------------- |

### Запрос на продажу недвижимости

```
TX
 * Buyer Users Id or Companies ID (JSON)
 * Buyer type (User or Company)
 * Property Id
 * Price (в валюте той страны, на территории котрой находится объект)
 * Подпись покупателя
```

Владалец недвижимости может иметь мультиподпись и хранить 2-й ключ в специальном органе, задача которого не допустить насильстенного воздействия на граждан с целью кражи их ищества. В таком случае, если Владалец недвижимости захочет совершить сделку, то ему нужно будет прийти в такое учреждение, назвать ID объекта недвижимости, подписать своим первым ключем спец. идентификационнй запрос, после чего он получит подпись, отправив её в сеть сделка будет совершена. Если продавец не боится, то может отключить необхолилмсть 2-й подписи.

###### PropertyRequests
| ID        | PropertyID  | BuyerUserId  | Price  | Status |
| ------------- | ------------- | ------------- | ------------- | ------------- |



Подверждение сделки продавом
```
TX
 * Buyer Users Id or Companies ID (JSON)
 * Buyer type (User or Company)
 * Property Id
 * Price (в валюте той страны, на территории котрой находится объект)
 * Подпись покупателя
```

###### PropertyRequestsAcceptHistory
| ID        | PropertyRequestsID  |  BlockId |
| ------------- | ------------- | ------------- |

### Расходные проводки


```
TX
 * Type (user|company)
 * Entries (JSON)
```

###### CreditEntries
| ID        | Entries(JSON)  |
| ------------- | ------------- |

Если компания хочет получить кредит, то она должна указать, на что будут потрачены средства.
Также проводки используются для верстки бюджета страны.


### Запрос на кредит

```
TX
 * Type (user|company)
 * EntryId
```

###### CreditsRequests
| ID        | EntryId  | Amount  | ModeratorId  | Result  |
| ------------- | ------------- | ------------- | ------------- | ------------- |


### Оформление наследства

```
TX
 * SmartCotract зашифрованный ключами наследников
 * Type зашифрованный или нет
 * Подпись расшированного смарт-контракта
 * UserId
 * Подпись отправителя
```

В случае смерти гражданина, становится возможным расшифровка и выполненеи его смарт-контракта, в котором описан алгоритм распределения наследства. 


###### Inheritance
| ID        | EncryptedSmartContract  | UserID  | SignatureDecryptedSmartContract  | DecryptedSmartContract  |  Status  |
| ------------- | ------------- | ------------- |------------- |------------- |------------- |

```
TX
 * Засшифрованный ключами наследников SmartCotract
 * UserId
 * Подпись отправителя
```
В расшифрованном смарт контракте есть подпись наследодателя, если она совпадает с той, что он отправил ранее (SignatureEncryptedSmartContract) то смарт-конракт выполняется.

### Регистрация брака

```
TX
 * Sender UserId
 * Recipient UserId
 * Брачнй контракт в виде Смарт-контракта
 * Подпись отправителя
```

Подверждение брака
```
TX
 * SpousesID
 * Подпись получателя запроса
```

###### Spouses
| ID        | SenderUserId  | RecipientUserId  | SmartContract  | Status  |
| ------------- | ------------- | ------------- | ------------- | ------------- |

###### SpousesRequestsAcceptHistory
| ID        |     SpousesId    |  Status  | BlockId |
| ------------- | ------------- | ------------- | ------------- |

Регистрация брака необходима для осуществления некоторых операций, в том числе последующего раздела имущества, в случае развода. Брачнй контракт - смарт контракт, который будет может быть выполнен только при статусе "разведены"


### Расторжение брака

Один супруг
```
TX
 * Spouses ID
 * SenderUserId
 * Подпись отправителя
```

Второй супруг
```
TX
 * Spouses ID
 * RecipientUserId
 * Подпись получателя
```

###### SpousesDivorce
| ID        |     SpousesId    |  Time1S1  | Time1S2  | Time2S1  | Time2S2  | Time1Close  | Time2Close  | 
| ------------- | ------------- | ------------- | ------------- |------------- |------------- |------------- |------------- |

Для расторжения брака необходимо отправить 2 раза по 2 транзакции с промежутком не менее 1 месяца. Для исключения импульсивных действий со стороны супругов. После расторжения брака для выполнения брачного контракта кто-то должен его расшифровать и отправить в сеть. При отсутствии контракта все имущество, приобретенное во время брака разделяется между супругамми.

##### Отмена расторжения брака
Один супруг
```
TX
 * Spouses ID
 * SenderUserId
 * Подпись отправителя
```

Второй супруг
```
TX
 * Spouses ID
 * RecipientUserId
 * Подпись получателя
```

Если супруги передумали разводиться, тогда они могут отправить отмену бракоразводного процесса. После этого появятся записи в Time1Close и Time2Close

### Брачный контракт

```
TX
 * SmartCotract
 * Подпись отправителя
```

В самом начале идет проверка статуса в таблице Spouses. Если там стоит "разведены", тогда происходит выполнение контракта. Например, все акции могут остаться за мужем, а недижимость перейдет к жене.



### Загрузка федерального бюджета

Расходы могут быть как явно указанными, например, зарплата конкретного сотрудника или закупка какого-то оборудования, так и ссылками на уже созданные Entries. Ссылки на Entries могут использоваться для перечисления средств каким-либо ведомствами или регионам.


```
TX
 * Entries (JSON)
Example: { "Payment": {"Period":"Monthly", "Type":"salary", "amount":"2000", "RecepientType", "User", "RecepientId": "6789419"}, "EntryId":168515 }
 * UserId главы государства
 * Подпись главы государства
```

###### AutoPayments
| ID        | Period  |Amount  |Type  | RecepientType  | RecepientId |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |

### Регистрация товаров

```
TX
 * CompanyId
 * Good name
 * Good Parametres (JSON)
 * Annual depreciation
```

###### Goods
| ID        | CompanyId  | GoodParametres  | AnnualAmortization  |
| ------------- | ------------- | ------------- | ------------- |

Ретейлер при продаже, например, айфона должен указать Good ID айфона, тогда покупатель будет знать, что он покупает именно айфон.  
Также, у товара указана амортизация, которая может быть учтена при автоматическом расчете налога компании.


### Регистрация Item компанией

```
TX
 * CompanyId
 * Name
 * Good ID (если это перепродажа товара)
 * Count of goods
 * Подпись ген. директора
```

###### Items
| ID        | CompanyId  | Name  | GoodId  | CountOfGoods  |
| ------------- | ------------- | ------------- | ------------- | ------------- |
Сделка по покупке какого-либо товара считается законной только при указании ID item. Это своего рода "чек", благодаря которому покупатель может пожаловаться на качество товара в соответствующий орган.
Item используется для составления ордеров. На ордеры выставлются счета.

### Периодичность выплаты зарплаты в компании
```
TX
 * ID компании
 * Периодичность в днях
 * Подпись ген. директора или доверенного лица
```

### Прием гражданина на работу
```
TX
 * ID гражданина
 * Должность
 * Зарплата
 * Подпись ген. директора или доверенного лица
```

###### Employees
| ID        | UserID  | Position  | Salary  | Date  |
| ------------- | ------------- | ------------- | ------------- | ------------- |


### Увольнение сотрудника
```
TX
 * ID сотрудника
 * Причина увольнения
 * Подпись ген. директора или доверенного лица
```

При увольнении, гражданину автоматически выплачивается выходное пособие. Размер пособия определяют органы местной власти.


### Начисление премии сотруднику
```
TX
 * ID сотрудника
 * Причина увольнения
 * Подпись ген. директора или доверенного лица
```

### Регистрация доверенного лица ген. директора
```
TX
 * ID сотрудника компании
 * Срок действия доверенности
 * Подпись ген. директора или доверенного лица
```

###### PowerOfAttorney
| ID        | EmployeeID  | CompanyID  |
| ------------- | ------------- | ------------- |

### Покупка товара компанией у компании

```
TX
 * CompanyId
 * Item ID или ID балансовой таблицы
 * Кол-во
 * Подпись ген. директора
```

Указание ID из балансовой таблицы нужно чтобы потом не проводить списание в ручном режиме.


###### BalanceCompany
| ID        | ItemID  | DateOfAdmission  |
| ------------- | ------------- | ------------- |

Указание ID товара нужно для того, чтобы на балансе компании числился конкретный товар. В случае ликвидации компании, акционеры получат доход от продажи имущества компании. Также при списании налогов учитывается амортизация, если у данного  Item ID она есть.

### Списание товара с баланса компании
```
TX
 * ID на балансе компании
 * Причина списания
 * Подпись ген. директора или доверенного лица
```

### Выписка счета

```
TX
 * Набор товаров (JSON)
 * Подпись кассира
```


###### CompanyOrders
| ID        | Items  | Time  |
| ------------- | ------------- | ------------- |

Покупатель приходит в магазин, набирает товаров,  кассир оправляет транзакцию со списком товаров, получает ID ордера, Покупатель показывает кассиру qr-код со воим userID, продавец выставлет счет для userID, покупатель отправляет транзакцию переволда средств, где шифрует своим ключём и ключём магазина ID ордера. Кассир видит платеж, где есть нужный ID ордера и отпускает покупателя. Весь процесс занимает несколько секунд. Информация о том, что именно купил покупатель есть только у него и у продавца.

###### CompanyInvoces
| ID        | UserId  | Amount  | CurrencyId  | Time | Status |
| ------------- | ------------- | ------------- | ------------- |------------- |------------- |


### Выпуск акции

```
TX
 * CompanyId
 * Shares {JSON}. Example {"UserId":146, "Shares": {"shares":100000, "privileges":1,3,4,6,8}}
```
 
###### Shares

| ID        | CompanyId  | Privileges  |
| ------------- | ------------- | ------------- |

###### OwnersOfShares

| ID        | UserId  | SharesId  | Amount  |
| ------------- | ------------- | ------------- | ------------- |

Все компании в OFS публичны. Торги акциями происходят на внутренней децентрализованной бирже. Акции можно наделить различными привилегиями. Что именно дают различные привилегии описывается в программном коде внутри LightDay.

### Ликвидация компании

```
TX
 * CompanyId
 * UserID
 * Vote
 * Подпись держателя голосующих акций
```

###### VotesLiquidationCompany

| ID        | UserId  |Vote |
| ------------- | ------------- | ------------- |

###### Auction

| ID        | GoodId  |Description |StartPrice |Step |EndPrice |Duration |
| ------------- |-------------|-------------|-------------|-------------|-------------|-------------|

Если акционеры решат ликвидировать компанию, тогда все средства на счету компании автоматически распределятся между акционерами, а имущество, находящееся на балансе компании выставляется на биржу.


### Покупка товаров на аукционе

```
TX
 * ID
 * Bet
 * Подпись пользователя
```

На аукционе можно продать или купить любые товары, которые имеют запись в таблице Items. 


### Buy/Sell акций

```
TX
 * ShareId
 * Price
 * Amount
 * CurrencyId
 * BuySell
 * Type (Company or User)
 * User ID or Company Id
 * Подпись пользователя или компании
```

###### SharesOrders
| ID        | UserId |  CompanyId | ShareId  | Price | Amount |  CurrencyId | BuySell | 
| ------------- |-------------|-------------|-------------|-------------|-------------|-------------|-------------|

На внутренней децентрализованной бирже акции компаний могут покупать любые пользователи из любой страны.

### Обмен валюты
```
TX
 * ShareId
 * Price
 * Amount
 * CurrencyId
 * Подпись пользователя
```

###### ForexOrders
| ID        | UserId | BuyCurrencyId  | Price | Amount |  SellCurrencyId |  EmptyBlockId | DelBlockId
| ------------- |-------------|-------------|-------------|-------------|-------------|-------------|-------------|



