---
description: >-
  Modify the output of translation, including the destination language and
  currency.
---

# Customizing Translation

The type of translation that can be performed is dependent on the values specified in the [translation request](./#sample-api-request). Below are guides on how to modify the translation to support your need.

{% tabs %}
{% tab title="Change Currency" %}
Given a numeric value of `23.23`,  it's impossible to identify what currency the above value stands for until a currency is attached to it.

To help the us better understand how to translate, it is required that you specify a **currency code** from our list of [supported ISO-417 currencies](../../supported-currencies.md#currency-codes).

**API Request**

To change currency of translation for [money to words API request](./#api-request), simply specify it the following body params:

* `currency`
{% endtab %}

{% tab title="Change Language" %}
Monetary values can be translated into just almost any language by passing it along with the request. 

To help the us better understand what to translate a monetary value into, it is required that you specify a **language code** from our list of [supported languages](../../supported-languages.md#language-codes).

**API Request**

To change language of translation for [money to words API request](./#api-request), simply specify it the following query params:

* `language`
{% endtab %}
{% endtabs %}









