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

### Samples

* [MQTTSample](https://github.com/IBMStreams/streamsx.mqtt/tree/develop/samples/MqttSample)
