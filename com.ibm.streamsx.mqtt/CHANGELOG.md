# Changes
==========
## v1.0.4:
* [#8](https://github.com/IBMStreams/streamsx.mqtt/issues/8) - I18n update

## v1.0.3:
* [#5](https://github.com/IBMStreams/streamsx.mqtt/issues/5) - set system property `com.ibm.jsse2.overrideDefaultTLS` to true, which removes the necessity to specify the **vmArg** parameter `"-Dcom.ibm.jsse2.overrideDefaultTLS=true"` to accept TLSv1.2.

## v1.0.2:
* [#3](https://github.com/IBMStreams/streamsx.mqtt/issues/3) - Update to latest snapshot version (v1.2.1) of Paho MQTT library, because of a reportet vulnerability.

## v1.0.1:
* Java sources removed from the release package.

## v1.0.0:
This is the first release of the MQTT toolkit.
It is a split-off from the Messaging toolkit version 5.3.4. You are encouraged to migrate from the messaging toolkit to this new toolkit. Read here, why and how to migrate.
Regarding the function, this release is identical with the MQTT part of the 5.3.4 release of the messaging toolkit.
