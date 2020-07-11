---
description: Translate monetary values into equivalent localized sentence.
---

# Localized Sentence

Any numeric value signifying an amount of money can easily be translated to the sentence equivalent in any _language of choice_.

To better understand the concept of translation, we've come up with a series of example that better explain it:

| Amount | Currency | Language | Translation |
| :--- | :--- | :--- | :--- |
| 2000 | `dollars`, `cents`  | English \(en\) | Two thousand dollars only. |
| 329.99 | `pounds`, `sterling`  | English \(en\) | Three hundred and twenty-nine pounds, ninety-nine sterling only. |
| 434103.34 | `naira`, `kobo` | English \(en\) | Four hundred and thirty-four thousand, one hundred and three naira, thirty-four kobo only. |

{% hint style="success" %}
**Customize:** To change the destination translation language, or currency, kindly check [customizing translation](customizing-translation.md).
{% endhint %}

### Sample API Request

{% api-method method="get" host="https://tuforty.com/api/v1" path="/translator/money" %}
{% api-method-summary %}
Get translation
{% endapi-method-summary %}

{% api-method-description %}
Translate money value into words
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer authentication token \(See Authentication\).
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="language" type="string" required=false %}
Language to translate into \(see supported languages\).
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" required=false %}
Money value to translate.
{% endapi-method-parameter %}

{% api-method-parameter name="whole\_unit" type="string" required=false %}
Unit to use for the whole part of the translation \(e.g. dollars\).
{% endapi-method-parameter %}

{% api-method-parameter name="decimal\_unit" type="string" required=false %}
Unit to use for the decimal part of the translation \(e.g. cent\)
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Full money value translation, alongside a complete breakdown of the whole and decimal parts.
{% endapi-method-response-example-description %}

```
{
    "whole_unit": "dollars",
    "decimal_unit": "cent",
    "language": "fr",
    "translation": "trois cent quarante-cinq dollars, trente-cinq cents seulement",
    "whole_translation": "Trois cent quarante cinq",
    "decimal_translation": "trente cinq"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=402 %}
{% api-method-response-example-description %}
Translation quota has been exhausted. Try purchasing a new quota.
{% endapi-method-response-example-description %}

```
{
    "message": "Not enough quota to perform this request."  
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=500 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "message": "An error occured; We've notified our dev team already."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



