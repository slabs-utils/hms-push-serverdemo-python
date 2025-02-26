## HMS PushKit Python Severdemo
English | [中文](https://github.com/HMS-Core/hms-push-serverdemo-python/blob/master/python37/README_ZH.md)

## Table of Contents

 * [Installation](#installation)
 * [Configuration ](#configuration )
 * [Sample Code](#sample-code)
 * [Libraries](#Libraries)
 * [License](#license)
 
 
	
## Installation

To install pushkit-python-sample, you should use pip:
```
pip install pip install -e "git+https://github.com/slabs-utils/hms-push-serverdemo-python.git@8aa574d582384dd837e3ae2955069e4225fce028#egg=huawei_push_admin&subdirectory=python37"

```


## Configuration 
The following table describes parameters of the initialize_app method.

| Parameter      |    Description |
| -------------  |   ------------------------------------------------------------------------- |
| appid          |    App ID, which is obtained from app information. |
| appsecret      |    Secret access key of an app, which is obtained from app information. |
| token_server   |    URL for the Huawei OAuth 2.0 service to obtain a token, please refer to [Generating an App-Level Access Token](https://developer.huawei.com/consumer/en/doc/development/parts-Guides/generating_app_level_access_token). |
| push_open_url  |    URL for accessing HUAWEI Push Kit, please refer to [Sending Messages](https://developer.huawei.com/consumer/en/doc/development/HMS-References/push-sendapi).||


## Sample Code
Download Python sample code in Downloading Server Sample Code.


Python sample code uses the Messaging structure in the push_admin package as the entry. Each method in the Messaging 
structure calls an API of the HUAWEI Push Kit server.

The following table describes methods in the Messaging structure.

| Method              |     Description
| -----------------   |     --------------------------------------------------- |
| send_message        |     Sends a message to a device. |
| subscribe_topic     |     Subscribes to a topic. |
| unsubscribe_topic   |     Unsubscribes from a topic. |
| list_topics         |     Queries the list of topics subscribed by a device. |
| initialize_app      |     Initializes the configuration parameters. |


1) Send an Android data message.
Code location: examples/send_data_message.py

2) Send an Android notification message.
Code location: examples/send_notify_message.py

3) Send a message by topic.
Code location: examples/send_topic_message.py

4) Send a message by conditions.
Code location: examples/send_condition_message.py

5) Send a message to a Huawei quick app.
Code location: examples/send_instance_app_message.py

6) Send a message through the WebPush agent.
Code location: examples/send_webpush_message.py

7) Send a message through the APNs agent.
Code location: examples/send_apns_message.py

8) Send a test message.
Code location: examples/send_test_message.py

## Libraries
| Library             |     Site
| -----------------   |     --------------------------------------------------- |
| requests            |     https://requests.readthedocs.io/en/master/ |
| six                 |     https://six.readthedocs.io/   |
## License

pushkit Python sample is licensed under the [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
