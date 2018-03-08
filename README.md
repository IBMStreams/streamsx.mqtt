# MQTT Toolkit

Welcome to the MQTT Toolkit. This toolkit enables SPL applications to integrate with MQTT servers.

## Why should you prefer this toolkit over the com.ibm.streamsx.messaging toolkit?

* This toolkit contains only the integration with MQTT and is very small compared with the messaging toolkit
* The MQTT function in the messaging toolkit is deprecated and will not be enhanced any more

## Migration from com.ibm.streamsx.messaging.mqtt

To migrate applications from the old MQTT operators in the `com.ibm.streamsx.messaging` toolkit, it is only required 
to make the SPL compiler aware of this toolkit and to change the SPL namespace of the used MQTT artifacts 
(operators, functions, and the like) in your SPL application. This toolkit includes everything in SPL namespace `com.ibm.streamsx.mqtt`,
while the MQTT function of the older `com.ibm.streamsx.messaging` toolkit uses the `com.ibm.streamsx.messaging.mqtt` namespace.

Operator names, function names, and the like are the same as in the messaging toolkit. The first release has no changes in the 
functionality compared with the [messaging toolkit version 5.3.4](https://github.com/IBMStreams/streamsx.messaging/releases/tag/v5.3.4).

## Releases

The MQTT Toolkit is offically released to support InfoSphere Streams v4.2:
* https://github.com/IBMStreams/streamsx.mqtt/releases

## Check out our SPLDOC here: 
* http://ibmstreams.github.io/streamsx.mqtt/com.ibm.streamsx.mqtt/doc/spldoc/html/index.html

## To get started with working with this toolkit

* https://github.com/IBMStreams/streamsx.mqtt/wiki/Getting-Started-with-Toolkit-Development
* [The messages and the NLS for toolkits](https://github.com/IBMStreams/administration/wiki/Messages-and-National-Language-Support-for-toolkits)


## To learn more about Streams

* [IBM Streams on Github](http://ibmstreams.github.io)
* [Introduction to Streams Quick Start Edition](http://ibmstreams.github.io/streamsx.documentation/docs/4.1/qse-intro/)
* [Streams Getting Started Guide](http://ibmstreams.github.io/streamsx.documentation/docs/4.1/qse-getting-started/)
* [StreamsDev](https://developer.ibm.com/streamsdev/)
