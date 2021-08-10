# Отчёт о тестировании Credit card number validator

## Краткое описание

10.08.2021 - 10.08.2021 было проведено Функциональное тестирование программы Credit card number validator.

На тестирование затрачено: 30 минут

В результате тестирования выявлены следующие дефекты:
* https://github.com/Manchester85/Java1/issues
* https://github.com/Manchester85/Java1/issues/2
* https://github.com/Manchester85/Java1/issues/3
* https://github.com/Manchester85/Java1/issues/4
* https://github.com/Manchester85/Java1/issues/5
* https://github.com/Manchester85/Java1/issues/6

## Описание процесса тестирования

В качестве тестовых данных использовались данные валидных карт, взятые на https://www.freeformatter.com/credit-card-number-generator-validator.html :
VISA:
4929522999531281    OK
4916270013381817112 FAIL – 19 numbers

MasterCard:
5303446272082205 OK
2221004709214994 OK

Maestro:
6763130222291238 OK
6304368985825778 OK

American Express (AMEX):
372350800740473 FAIL 15 numbers
343914921175699 FAIL 15 numbers

Discover:
6011356660529066 OK
6011539447295690121 FAIL 19 numbers

JCB:
3529095727915999 OK 
3528100058057875761 FAIL 19 numbers

Diners Club - North America:
5429207020155241 OK
5560451068629449 OK

Diners Club - Carte Blanche:
30432103344684 FAIL 14 numbers
30590826618245 FAIL 14 numbers 

Diners Club - International:
36610924061629 FAIL 14 numbers
36416281555835 FAIL 14 numbers

Visa Electron:
4844717121781919 OK
4508238344549501 OK

InstaPayment:
6370485041256290 OK
6374791285004098 OK

Тестирование производилось в следующем окружении:
* Windows 10, 64 бит
* JAVA version "11.0.11" 2021-04-20

