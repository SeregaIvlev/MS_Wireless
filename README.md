# MS_Wireless
Microsat wireless board software


Протокол обмена SPI:
1) В начале опускается нога SPI, поднимать желательно только после окончания сессии обмена. Дополнительные задние фронты не допускаются.
2) Первым байтом передаётся запрос:
Значение 0: только получение данных с радио
Значения 1-32: передача данных на землю
Значения >32: получение данных с gps.
