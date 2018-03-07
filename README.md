# MQTT Toolkit

Welcome to the MQTT Toolkit. This toolkit enables SPL applications to integrate with MQTT servers.

## Migration from com.ibm.streamsx.messaging.mqtt

To migrate applications from the old MQTT operators in the `com.ibm.streamsx.messaging` toolkit, it is only required 
to make the SPL compiler aware of this toolkit and to change the SPL namespace of the used MQTT artifacts 
(operators, functions, and the like) in your SPL application. The `com.ibm.streamsx.messaging` toolkit uses the 
namespace `com.ibm.streamsx.messaging.mqtt`, this toolkit includes everything in namespace `com.ibm.streamsx.mqtt`. 
Operator names, function names, and the like are the same as in the messaging toolkit. There are no changes in the 
functionality compared with the [messaging toolkit version 5.3.4](https://github.com/IBMStreams/streamsx.messaging/releases/tag/v5.3.4).

## Releases

coming soon
