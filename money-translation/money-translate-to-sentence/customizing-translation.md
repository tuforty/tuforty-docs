---
description: >-
  Modify the output of translation, including the destination language and
  currency.
---

# Customizing Translation

The type of translation that can be performed is dependent on the values specified in the [translation request](./#sample-api-request). Below are guides on how to modify the translation to support your need.

{% tabs %}
{% tab title="Change Currency" %}
Given a numeric value of `23.23`, it's impossible to identify what currency the above value stands for. To help the us better understand how to translate, it is required that you specify the currency. 

#### Changing Currency

A currency can best be understood by providing the units for:

* whole number \(e.g. `dollars`, `pounds`\)
* decimal number \(e.g. `cents`, `sterling`\)

### API Request

To change currency of translation if [money to words API request](./#api-request), simply specify it the following body params:

* `whole_unit` 
* `decimal_unit`
{% endtab %}

{% tab title="Change Language" %}
It is possible to specify what language to translate the into. 

This requires specifying the language **abbreviation** in the **language** query param.

{% hint style="success" %}
**Supported Languages:** For supported abbreviations, kindly check [supported languages.](../../supported-languages.md#language-abbreviations)
{% endhint %}
{% endtab %}
{% endtabs %}



