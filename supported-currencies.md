---
description: Currencies we support for money values.
---

# 💰Supported Currencies

We currently support all [ISO-4217](https://en.wikipedia.org/wiki/ISO_4217) currencies and official fractional units, which spans over **165+** in total. Each money translation to be performed requires that a currency is specified, which directly gives the number a monetary value.

{% hint style="info" %}
**Notice:** In the API, you'll be required to use the **code** of each currency.
{% endhint %}

### 

### Supported Currencies \(API\)

{% api-method method="get" host="https://tuforty.com/api/v1" path="/supported/currencies" %}
{% api-method-summary %}
Get supported currencies
{% endapi-method-summary %}

{% api-method-description %}
Get a list of all supported currencies
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
[
    "RUB",
    "EUR",
    "GBP",
    "GGP",
    "DZD",
    "XCD",
    "AMD",
    "SHP",
    "XOF",
    "AUD",
    "INR",
    "USD",
    "BND",
    "SGD",
    "XAF",
    "NZD",
    "ANG",
    "DKK",
    "ZAR",
    "XPF",
    "ILS",
    "JOD",
    "MRU",
    "CHF",
    "MAD",
    "TRY",
    "AFN",
    "ALL",
    "AOA",
    "ARS",
    "AWG",
    "AZN",
    "BSD",
    "BHD",
    "BDT",
    "BBD",
    "BYN",
    "BZD",
    "BMD",
    "BTN",
    "BOB",
    "BWP",
    "BRL",
    "BGN",
    "BIF",
    "KHR",
    "CAD",
    "CVE",
    "KYD",
    "CLP",
    "CNY",
    "COP",
    "KMF",
    "CDF",
    "CKD",
    "CRC",
    "HRK",
    "CUP",
    "CZK",
    "DJF",
    "DOP",
    "EGP",
    "ERN",
    "SZL",
    "ETB",
    "FKP",
    "FOK",
    "FJD",
    "GMD",
    "GEL",
    "GHS",
    "GIP",
    "GTQ",
    "GNF",
    "GYD",
    "HTG",
    "HNL",
    "HKD",
    "HUF",
    "ISK",
    "IDR",
    "IRR",
    "IQD",
    "IMP",
    "JMD",
    "JPY",
    "JEP",
    "KZT",
    "KES",
    "KID",
    "KPW",
    "KRW",
    "KWD",
    "KGS",
    "LAK",
    "LBP",
    "LSL",
    "LRD",
    "LYD",
    "MOP",
    "MGA",
    "MWK",
    "MYR",
    "MVR",
    "MUR",
    "MXN",
    "MDL",
    "MNT",
    "MZN",
    "MMK",
    "NAD",
    "NPR",
    "NIO",
    "NGN",
    "MKD",
    "NOK",
    "OMR",
    "PKR",
    "PAB",
    "PGK",
    "PYG",
    "PEN",
    "PHP",
    "PND",
    "PLN",
    "QAR",
    "RON",
    "RWF",
    "WST",
    "STN",
    "SAR",
    "RSD",
    "SCR",
    "SLL",
    "SBD",
    "SOS",
    "SLS",
    "SSP",
    "LKR",
    "SDG",
    "SRD",
    "SEK",
    "SYP",
    "TWD",
    "TJS",
    "TZS",
    "THB",
    "TOP",
    "PRB",
    "TTD",
    "TND",
    "TMT",
    "TVD",
    "UGX",
    "UAH",
    "AED",
    "UYU",
    "UZS",
    "VUV",
    "VES",
    "VND",
    "YER",
    "ZMW",
    "ZWL",
    "CUC",
    "BAM"
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## Currency Codes

| Currency | Code |  | Currency | Code |
| :--- | :--- | :--- | :--- | :--- |
| Afghan afghani | **AFN** |  | Lesotho loti | **LSL** |
| Albanian lek | **ALL** |  | Liberian dollar | **LRD** |
| Algerian dinar | **DZD** |  | Libyan dinar | **LYD** |
| Angolan kwanza | **AOA** |  | Macanese pataca | **MOP** |
| Argentine peso | **ARS** |  | Macedonian denar | **MKD** |
| Armenian dram | **AMD** |  | Malagasy ariary | **MGA** |
| Aruban florin | **AWG** |  | Malawian kwacha | **MWK** |
| Australian dollar | **AUD** |  | Malaysian ringgit | **MYR** |
| Azerbaijani manat | **AZN** |  | Maldivian rufiyaa | **MVR** |
| Bahamian dollar | **BSD** |  | Manx pound | **IMP** |
| Bahraini dinar | **BHD** |  | Mauritanian ouguiya | **MRU** |
| Bangladeshi taka | **BDT** |  | Mauritian rupee | **MUR** |
| Barbadian dollar | **BBD** |  | Mexican peso | **MXN** |
| Belarusian ruble | **BYN** |  | Moldovan leu | **MDL** |
| Belize dollar | **BZD** |  | Mongolian tögrög | **MNT** |
| Bermudian dollar | **BMD** |  | Moroccan dirham | **MAD** |
| Bhutanese ngultrum | **BTN** |  | Mozambican metical | **MZN** |
| Bolivian boliviano | **BOB** |  | Namibian dollar | **NAD** |
| Bosnia and Herzegovina convertible mark | **BAM** |  | Nepalese rupee | **NPR** |
| Botswana pula | **BWP** |  | Netherlands Antillean guilder | **ANG** |
| Brazilian real | **BRL** |  | New Taiwan dollar | **TWD** |
| British pound | **GBP** |  | New Zealand dollar | **NZD** |
| Brunei dollar | **BND** |  | Nicaraguan córdoba | **NIO** |
| Bulgarian lev | **BGN** |  | Nigerian naira | **NGN** |
| Burmese kyat | **MMK** |  | North Korean won | **KPW** |
| Burundian franc | **BIF** |  | Norwegian krone | **NOK** |
| Cambodian riel | **KHR** |  | Omani rial | **OMR** |
| Canadian dollar | **CAD** |  | Pakistani rupee | **PKR** |
| Cape Verdean escudo | **CVE** |  | Panamanian balboa | **PAB** |
| Cayman Islands dollar | **KYD** |  | Papua New Guinean kina | **PGK** |
| Central African CFA franc | **XAF** |  | Paraguayan guaraní | **PYG** |
| CFP franc | **XPF** |  | Peruvian sol | **PEN** |
| Chilean peso | **CLP** |  | Philippine peso | **PHP** |
| Chinese yuan | **CNY** |  | Pitcairn Islands dollar | **PND** |
| Colombian peso | **COP** |  | Polish złoty | **PLN** |
| Comorian franc | **KMF** |  | Qatari riyal | **QAR** |
| Congolese franc | **CDF** |  | Romanian leu | **RON** |
| Cook Islands dollar | **CKD** |  | RTGS dollar | **ZWL** |
| Costa Rican colón | **CRC** |  | Russian ruble | **RUB** |
| Croatian kuna | **HRK** |  | Rwandan franc | **RWF** |
| Cuban convertible peso | **CUC** |  | Saint Helena pound | **SHP** |
| Cuban peso | **CUP** |  | Samoan tālā | **WST** |
| Czech koruna | **CZK** |  | São Tomé and Príncipe dobra | **STN** |
| Danish krone | **DKK** |  | Saudi riyal | **SAR** |
| Djiboutian franc | **DJF** |  | Serbian dinar | **RSD** |
| Dominican peso | **DOP** |  | Seychellois rupee | **SCR** |
| Eastern Caribbean dollar | **XCD** |  | Sierra Leonean leone | **SLL** |
| Egyptian pound | **EGP** |  | Singapore dollar | **SGD** |
| Eritrean nakfa | **ERN** |  | Solomon Islands dollar | **SBD** |
| Ethiopian birr | **ETB** |  | Somali shilling | **SOS** |
| Euro | **EUR** |  | Somaliland shilling | **SLS** |
| Falkland Islands pound | **FKP** |  | South African rand | **ZAR** |
| Faroese króna | **FOK** |  | South Korean won | **KRW** |
| Fijian dollar | **FJD** |  | South Sudanese pound | **SSP** |
| Gambian dalasi | **GMD** |  | Sri Lankan rupee | **LKR** |
| Georgian lari | **GEL** |  | Sudanese pound | **SDG** |
| Ghanaian cedi | **GHS** |  | Surinamese dollar | **SRD** |
| Gibraltar pound | **GIP** |  | Swazi lilangeni | **SZL** |
| Guatemalan quetzal | **GTQ** |  | Swedish krona | **SEK** |
| Guernsey pound | **GGP** |  | Swiss franc | **CHF** |
| Guinean franc | **GNF** |  | Syrian pound | **SYP** |
| Guyanese dollar | **GYD** |  | Tajikistani somoni | **TJS** |
| Haitian gourde | **HTG** |  | Tanzanian shilling | **TZS** |
| Honduran lempira | **HNL** |  | Thai baht | **THB** |
| Hong Kong dollar | **HKD** |  | Tongan paʻanga | **TOP** |
| Hungarian forint | **HUF** |  | Transnistrian ruble | **PRB** |
| Icelandic króna | **ISK** |  | Trinidad and Tobago dollar | **TTD** |
| Indian rupee | **INR** |  | Tunisian dinar | **TND** |
| Indonesian rupiah | **IDR** |  | Turkish lira | **TRY** |
| Iranian rial | **IRR** |  | Turkmenistan manat | **TMT** |
| Iraqi dinar | **IQD** |  | Tuvaluan dollar | **TVD** |
| Israeli new shekel | **ILS** |  | Ugandan shilling | **UGX** |
| Jamaican dollar | **JMD** |  | Ukrainian hryvnia | **UAH** |
| Japanese yen | **JPY** |  | United Arab Emirates dirham | **AED** |
| Jersey pound | **JEP** |  | United States dollar | **USD** |
| Jordanian dinar | **JOD** |  | Uruguayan peso | **UYU** |
| Kazakhstani tenge | **KZT** |  | Uzbekistani soʻm | **UZS** |
| Kenyan shilling | **KES** |  | Vanuatu vatu | **VUV** |
| Kiribati dollar | **KID** |  | Venezuelan bolívar soberano | **VES** |
| Kuwaiti dinar | **KWD** |  | Vietnamese đồng | **VND** |
| Kyrgyzstani som | **KGS** |  | West African CFA franc | **XOF** |
| Lao kip | **LAK** |  | Yemeni rial | **YER** |
| Lebanese pound | **LBP** |  | Zambian kwacha | **ZMW** |





