---                             
title: "MOCKABLE_FUNCTION function reference | Microsoft Docs" 
titleSuffix: "Azure IoT C SDK"            
description: "This is the function reference page for the MOCKABLE_FUNCTION() function in the Azure IoT C SDK. This SDK is used with Azure IoT Hub and Azure IoT Hub Device Provisioning Service"            
manager: timlt                 
author: wesmc7777              
ms.author: wesmc               
ms.date: 09/23/2020                    
ms.service: "iot-hub"             
ms.custom: ""                
ms.topic: "reference"        
---                            

# MOCKABLE_FUNCTION()

IoTHubClient_Init Initializes the IoTHub Client System.

## Syntax

\#include "[azure-iot-sdk-c/iothub_client/inc/iothub.h](../iothub-h.md)"  
```C
MOCKABLE_FUNCTION(
  int,
  IoTHub_Init
);
```

## Return Value
int zero upon success, any other value upon failure.
