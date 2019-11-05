# siot of mPython

SIoT means Science and Simple Internet of Things.<br>
SIoT focuses on the collection and export of IoT data and is one of the best choices for collecting scientific data.<br>
DFRobot provide a solution of SIoT on python and mpython.<br>

## Table of Contents

* [Summary](#summary)
* [Installation](#installation)
* [Methods](#methods)
* [Compatibility](#compatibility)
* [Credits](#credits)
<snippet>
<content>

## Summary
You need to build an mqtt server first.<br>
Then input the information of mqtt server.<br>

## Installation

Clone this library and run the example on Python and mpython.<br>
The other way,imput"pip3 siot"on Python and run example.<br>

## Methods
```Python
'''
#@brief input the information of mqtt server
#@param client_id:client_id can be null
#       server:MQTT server IP address
#       user:IOT_UserName
#       password:IOT_PassWord
def init(client_id, server, port=0, user=None, password=None, keepalive=0,ssl=False, ssl_params={})
'''

'''
#@brief set callback function 
#@param f:function set by users
def set_callback(f)
'''

'''
#@brief send message to server 
#@param topic:ID of device
#       callback:callback function of set_callback(f)
def subscribe(topic, callback)
'''

'''
#@brief connect server and device
def connect()
'''

'''
#@brief repeat detect if data is received
def loop()
'''

'''
#@brief disconnect the server
def stop()
'''

'''
#@brief repeat detect if data is received
#@param topic:ID of device
#       msg:data to publish
def publish(topic, msg, retain=False, qos=0)
'''

'''
#@brief send message to server 
#@param topic:ID of device
def getsubscribe(topic, qos=0)
'''
```
## Credits

·author [luoyufeng yufeng.luo@dfrobot.com]
