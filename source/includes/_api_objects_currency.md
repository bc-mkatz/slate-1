# <span class="jumptarget"> Currency Reference </span>

The Currency object and endpoints manage alternate currency display options on the storefront.

## <span class="jumptarget"> Currency Object – Properties </span>

| Name | Type | Description |
|---|---|---|
| id | int | The ID of the currency. Read-only. |
| is_default | boolean | Specifies whether this is the store's default currency display format. Read-only. | 
| date_created | date | Date on which this currency was created on the store. |
| date_modified | date | Date on which this currency was last modified on the store. |
| country_iso2 | string | 2-letter [ISO Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) code for this currency's country. |
| currency_code | string | 3-letter [ISO 4217 code](http://www.xe.com/iso4217.php) for this currency. |
| currency_exchange_rate | float | Amount of this currency that is equivalent to one U.S. dollar. |
| auto_update | boolean | Specifies whether to use the [XE Currency Converter](http://www.xe.com/currencyconverter/) service to update the currency conversion. A value of `false` specifies a static conversion value. |
| location | string | Specifies whether this currency's symbol appears to the "left" or "right" of the numeric amount. |
| token | string | Symbol for this currency. |
| decimal_token | string | Symbol used as the decimal separator in this currency. |
| thousands_token | string | Symbol used as the thousands separator in this currency. |
| decimal_places | int | Number of decimal places to show for this currency. |
