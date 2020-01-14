# mqttlights
## mqtt python appservice to serial gateway

## Mqtt service application on Raspberry pi
- maps mqtt topics to serial communications to Arduino

## Serial
  - /dev/ttyUSB0
  - 9600

# Provided mqtt command Topics
```
- home/mqttlights/ulkovalot
- home/mqttlights/ykaula
- home/mqttlights/veranta
- home/mqttlights/ykmh
- home/mqttlights/ykph
```
# Provided mqtt state Topics
```
- home/mqttlights/ulkovalot/state
- home/mqttlights/ykaula/state
- home/mqttlights/veranta/state
- home/mqttlights/ykmh/state
- home/mqttlights/ykph/state
```
state query sends state query to serial 
```
            Query:                   Response:
--------------------------------------------------------
veranta     1state                   1state:1 or 1state:0
parvekepr   2state                   2state:1 or 2state:0
ykaula      3state                   3state:1 or 3state:0
ulkovalot   4state                   4state:1 or 4state:0
ykmh        5state                   5state:1 or 5state:0
ykph        6state                   6state:1 or 6state:0
```
Arduino responds room and the state ON/OFF and switches the GPIO accordingly
```
          Query:                     Response:
--------------------------------------------------------
veranta     1setON or 1setOFF        1state:ON or 1state:OFF                                         
parvekepr   2setON or 2setOFF        2state:ON or 2state:OFF
ykaula      3setON or 3setOFF        3state:ON or 3state:OFF
ulkovalot   4setON or 4setOFF        4state:ON or 4state:OFF
ykmh        5setON or 5setOFF        5state:ON or 5state:OFF
ykph        6setON or 6setOFF        6state:ON or 6state:OFF
```



