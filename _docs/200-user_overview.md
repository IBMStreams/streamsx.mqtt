---
title: "Toolkit Usage Overview"
permalink: /docs/user/overview/
excerpt: "How to use this toolkit."
last_modified_at: 2018-02-22T12:37:48+01:00
redirect_from:
   - /theme-setup/
sidebar:
   nav: "userdocs"
---
{% include toc %}
{%include editme %}

The MQTT toolkit contains two operators, the *MQTTSink*, and the *MQTTSource*.
The MQTTSink operator creates publishes MQTT messages to MQTT topics from tuples and acts therefore
as a sink operator within your Streams application.

The MQTTSource operator subscribes to MQTT topics and consumes messages. It creates Tuples which are processed by
other downstream operators of the Streams application. It is a source operator within your Streams application.

For both, the MQTTSink and the MQTTSource there is a one-to-one relationship between tuples and MQTT messages.
Read more about how to use these operators in the [SPL documentaion](/streamsx.mqtt/doc/spldoc/html/index.html).


### Why should you prefer this toolkit over the com.ibm.streamsx.messaging toolkit?

* This toolkit contains only the integration with MQTT and is very small compared with the messaging toolkit, 
  which contains operators for various messaging systems.
* The MQTT function in the messaging toolkit is deprecated and will not be enhanced any more.


### Migration from the MQTT operators in the com.ibm.streamsx.messaging toolkit

To migrate applications from the old MQTT operators in the `com.ibm.streamsx.messaging` toolkit, it is only required
to make the SPL compiler aware of this toolkit and to change the SPL namespace of the used MQTT artifacts
(operators, functions, and the like) in your SPL application. This toolkit includes everything in SPL namespace 
`com.ibm.streamsx.mqtt`, while the MQTT function of the older `com.ibm.streamsx.messaging` toolkit uses the 
`com.ibm.streamsx.messaging.mqtt` namespace.

Operator names, function names, and the like are the same as in the messaging toolkit. The first release has no changes in the
functionality compared with the [messaging toolkit version 5.3.4](https://github.com/IBMStreams/streamsx.messaging/releases/tag/v5.3.4).


### Samples

* [MQTTSample](https://github.com/IBMStreams/streamsx.mqtt/tree/develop/samples/MqttSample)
