# Copyright (C)2016, International Business Machines Corporation and  
# others. All Rights Reserved.                        
.PHONY: all clean

STREAMS_MQTT_TOOLKIT ?= ../../com.ibm.streamsx.mqtt:${STREAMS_INSTALL}/toolkits/com.ibm.streamsx.mqtt

SPLC_FLAGS ?= -a -t ${STREAMS_MQTT_TOOLKIT} --data-directory=data

SPLC = $(STREAMS_INSTALL)/bin/sc

SPL_CMD_ARGS ?=
SPL_MAIN_COMPOSITE = application::MqttSample
OUTPUT_DIR = output

all: 
	$(SPLC) $(SPLC_FLAGS) -M $(SPL_MAIN_COMPOSITE) --output-dir ./$(OUTPUT_DIR) $(SPL_CMD_ARGS)

clean:
	$(SPLC) $(SPLC_FLAGS) -C -M $(SPL_MAIN_COMPOSITE)


