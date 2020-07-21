---
description: Translate monetary values into equivalent localized sentence.
---

# Localized Sentence

Any numeric value signifying an amount of money can easily be translated to the sentence equivalent in any _language of choice_.

To better understand the concept of translation, we've come up with a series of example that better explain it:

| Amount | Currency | Language | Translation |
| :--- | :--- | :--- | :--- |
| 2000 | `USD`  | English \(`en`\) | Two thousand dollars only. |
| 329.99 | `GBP`  | English \(`en`\) | Three hundred and twenty-nine pounds, ninety-nine sterling only. |
| 329.99 | `GBP` | French \(`fr`\) | trois cent vingt-neuf livres, quatre-vingt-dix-neuf penny seulement |
| 434103.34 | `NGN` | English \(`en`\) | Four hundred and thirty-four thousand, one hundred and three naira, thirty-four kobo only. |
| 八百七十二万七千八百二十四 | `USD` | English \(`en`\) | Twenty-four dollar, forty-five cent only |
| 八百七十二万七千八百二十四 | `GBP` | Arabic \(`ar`\) | أربعة وعشرون نيرة ، خمسة وأربعون كوبو فقط |

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
{% api-method-parameter name="value" type="string" required=true %}
Money value to translate \(must be equal or greater than zero\).
{% endapi-method-parameter %}

{% api-method-parameter name="currency" type="string" required=true %}
Currency to use for the value specified \(e.g. GBP, USD, INR\).
{% endapi-method-parameter %}

{% api-method-parameter name="language" type="string" required=true %}
Language to translate into \(see supported languages\).
{% endapi-method-parameter %}

{% api-method-parameter name="use\_short" type="boolean" required=false %}
Use shorter form of a currency to generate a  a translation.  
  
**Example:**  
Given the currency **CAD**, the:  
- short form is **Dollar** & **Cent**  
- long form  is **Canadian Dollar** & **Cent**  
  
By default, **use\_short** is **true**.
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
    "whole_unit": "pound",
    "decimal_unit": "penny",
    "language": "fr",
    "currency": "GBP",
    "translation": "trois cent vingt-neuf livres, quatre-vingt-dix-neuf penny seulement",
    "whole_translation": "trois cent vingt-neuf",
    "decimal_translation": "quatre-vingt-dix-neuf"
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



