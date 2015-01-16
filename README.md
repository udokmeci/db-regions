# db-regions
This repository has basic regional data for to be used and adopted easily and welcomes any contribution to be used in my and your next project.

For now only MySQL dump all we have. Hope there will be more with contributions.

**Notice:** You have to add countires tables first since all other tables are depended on it otherwise you should change SQL files to remove dependencies.

## Countriues
If you like to add countires please add `{db}/countries/countries.sql` file first. Then you can also add i18n to get names in different languages.

## Cities
If you like to add cities for some countries please add `{db}/cities/{country_code}_cities.sql` files. If you like to add all once, use  `{db}/cities/_all.sql`
**Notice:** There are very dirty and duplicate entries in all countries. I will add an issue for such files. And if there is none for the one you find please add a new issue.

## Currencies
`{db}/currencies/currency.sql` is the file you look for. E is the number of decimal places used for currency.

### Currencies of Countries
There is also a file `{db}/currencies/country_currency.sql` under `currencies` folder which gives you the pivot table of the relation of currencies used in countries.

## Contribution
`Cities` has many problems. Some of them are duplicate and missing. I have tried to fix as much as possible however there is too much to go. Please help and let all use such data for free. 
### Cities
Please do not change `uid` when updating however you can add new lines with `uid` like uppercase `country_code` and `6 digit random string`.

`uid` data will be used for patching the updates.

##Why?
I have started for this kind of data since I had to work on a project which offers PayPal payment.

``` php
State is required
```
Exception is why I have started. Data is now properly adjusted with the [given here](https://developer.paypal.com/docs/classic/api/state_codes/). Except `Armed Forces APO` and `Outlying Areas`. Also all the cities I have found for countries listed [here](https://developer.paypal.com/docs/classic/api/merchant/DoDirectPayment_API_Operation_NVP/) (see: `SHIPTOSTATE`). 

Thank you for using and contributing. Hope it will save some time that I have lost.

## Safe to Use?

Some countries are good to go.

 - Argentina
 - Austria
 - Brazil
 - Canada
 - China
 - Germany
 - India
 - Indonesia
 - Italy
 - Japan
 - Mexico
 - Netherlands
 - Thailand
 - Turkey
 - United States




