# TwinCAT_Tibber

An example how to fetch today and tomorrows electricity price from Tibber.
Use it as is and for free. No warranty.

Based on the Beckhoff HTTP REST Postman POST exampple:
https://infosys.beckhoff.com/content/1033/tf6760_tc3_iot_https_rest/7645683851.html?id=4299616368702372088

Here you can test other querys:
https://developer.tibber.com/explorer

Postman is another great tool for testing:
https://www.postman.com/

HTTPS REST is supported from TwinCAT3 4024.7. One CX9020 with 4024.7 did not work with the Tibber example. Tested and working on 4024.22 and above.

Tibber demo token is included. Just run the funcktion block and you should get the electricity prices in an array of struct. Change sToken input to your personal Token, provided by Tibber.
The struct is done for the included querys. For new querys, make proper adjustment to the struct. And querys to the method in the function block and make propper adjustment to en Enum, E_Query.
PS. Tibber release tomorrows prices after 13:00. Before then you must ask for todays prices to get a reslut.

Kind regards Fredrik
