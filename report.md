# Отчёт о тестировании Credit card number validator

## Краткое описание

10.08.2021 - 10.08.2021 было проведено Функциональное тестирование программы Credit card number validator.

На тестирование затрачено: 50 минут

В результате тестирования выявлены следующие дефекты:
**[Валидатор карт ошибочно выдает результат FAIL при вводе 19-значных валидных номеров карт VISA](https://github.com/Manchester85/Java1/issues)**.
**[Валидатор карт ошибочно выдает результат FAIL при вводе 15-значных валидных номеров карт AMEX](https://github.com/Manchester85/Java1/issues/2)**.
**[Валидатор карт ошибочно выдает результат FAIL при вводе 19-значных валидных номеров карт Discover](https://github.com/Manchester85/Java1/issues/3)**.
**[Валидатор карт ошибочно выдает результат FAIL при вводе 19-значных валидных номеров карт JCB](https://github.com/Manchester85/Java1/issues/4)**.
**[Валидатор карт ошибочно выдает результат FAIL при вводе 14-значных валидных номеров карт Diners Club - Carte Blanche](https://github.com/Manchester85/Java1/issues/5)**.
**[Валидатор карт ошибочно выдает результат FAIL при вводе 14-значных валидных номеров карт Diners Club International](https://github.com/Manchester85/Java1/issues/6)**.

## Описание процесса тестирования

В качестве тестовых данных использовались данные валидных карт, взятые на **[card data](https://www.freeformatter.com/credit-card-number-generator-validator.html)**. :
**VISA**:
4929522999531281    OK
4916270013381817112 FAIL 19 numbers
4173029165083247691 FAIL 19 numbers
4539043282587113628 FAIL 19 numbers

**MasterCard**:
5303446272082205 OK
2221004709214994 OK
5586830710331415 OK
5280166915038961 OK

**Maestro**:
6763130222291238 OK
6304368985825778 OK
5038786142800266 OK 
6762557864806058 OK

**American Express(AMEX)**:
372350800740473 FAIL 15 numbers
343914921175699 FAIL 15 numbers
347665457977660 FAIL 15 numbers
343500108280343 FAIL 15 numbers

**Discover**:
6011356660529066 OK
6011539447295690121 FAIL 19 numbers
6011893531397908232 FAIL 19 numbers
6011198652944865626 FAIL 19 numbers

**JCB**:
3529095727915999 OK 
3528100058057875761 FAIL 19 numbers
3528700587880446246 FAIL 19 numbers
3541153300914481378 FAIL 19 numbers 

**Diners Club - North America**:
5429207020155241 OK
5560451068629449 OK
5421376443055540 OK
5543102913416134 OK

**Diners Club - Carte Blanche**:
30432103344684 FAIL 14 numbers
30590826618245 FAIL 14 numbers 
30378887915092 FAIL 14 numbers
30425593048815 FAIL 14 numbers

**Diners Club - International**:
36610924061629 FAIL 14 numbers
36416281555835 FAIL 14 numbers
36449029862940 FAIL 14 numbers
36505030999979 FAIL 14 numbers

**Visa Electron**:
4844717121781919 OK
4508238344549501 OK
4508054927446316 OK
4917407437714257 OK

**InstaPayment**:
6370485041256290 OK
6374791285004098 OK
6390609929340837 OK
6397602555684134 OK


### Тестирование производилось в следующем окружении:
* Windows 10, 64 бит
* JAVA version "11.0.11" 2021-04-20

