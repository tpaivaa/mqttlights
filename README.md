### mqttlights
#mqtt python appservice to serial gateway

##Mqtt service application on Raspberry pi
- maps mqtt topics to serial communications to Arduino

# Serial
  - /dev/ttyUSB0
  - 9600

#Provided mqtt command Topics

home/mqttlights/ulkovalot
home/mqttlights/ykaula
home/mqttlights/veranta
home/mqttlights/ykmh
home/mqttlights/ykph

#Provided mqtt state Topics

home/mqttlights/ulkovalot/state
home/mqttlights/ykaula/state
home/mqttlights/veranta/state
home/mqttlights/ykmh/state
home/mqttlights/ykph/state

state query sends state query to serial 
ulkovalot   1state
ykaula      2state
veranta     3state
ykmh        4state
ykph        5state

Arduino responds room and the state ON/OFF




