---                             
title: "iothub_client_core.h header file reference | Microsoft Docs" 
titleSuffix: "Azure IoT C SDK"            
description: "This is the header file reference page for iothub_client_core.h in the Azure IoT C SDK. This SDK is used with Azure IoT Hub and Azure IoT Hub Device Provisioning Service"            
manager: timlt                 
author: wesmc7777              
ms.author: wesmc               
ms.date: 10/24/2018                    
ms.service: "iot-hub"             
ms.custom: ""                
ms.topic: "reference"        
---                            

# iothub_client_core.h 

Extends the IoTHubClientCore_LL module with additional features.

## Includes

\#include <stddef.h>  
\#include <stdint.h>  
\#include "[azure_c_shared_utility/umock_c_prod.h](umock-c-prod-h.md)"  
\#include "[iothub_client_core_ll.h](iothub-client-core-ll-h.md)"  

## Detailed Description

IoTHubClientCore is a module that extends the IoTHubClientCore_LL module with 2 features:

* scheduling the work for the IoTHubCLient from a thread, so that the user does not need to create their own thread

* thread-safe APIs

This is an internal APIs used by the Azure IoT C SDK to communicate with an Azure IoTHub.

Direct use of this library header is not supported.

## Functions

Function Name                  | Description                                
--------------------------------|---------------------------------------------
[IoTHubClientCore_CreateFromConnectionString](./iothub-client-core-h/iothubclientcore-createfromconnectionstring.md)            | 
[IoTHubClientCore_Create](./iothub-client-core-h/iothubclientcore-create.md)            | 
[IoTHubClientCore_CreateWithTransport](./iothub-client-core-h/iothubclientcore-createwithtransport.md)            | 
[IoTHubClientCore_CreateFromDeviceAuth](./iothub-client-core-h/iothubclientcore-createfromdeviceauth.md)            | 
[IoTHubClientCore_Destroy](./iothub-client-core-h/iothubclientcore-destroy.md)            | 
[IoTHubClientCore_SendEventAsync](./iothub-client-core-h/iothubclientcore-sendeventasync.md)            | 
[IoTHubClientCore_GetSendStatus](./iothub-client-core-h/iothubclientcore-getsendstatus.md)            | 
[IoTHubClientCore_SetMessageCallback](./iothub-client-core-h/iothubclientcore-setmessagecallback.md)            | 
[IoTHubClientCore_SetConnectionStatusCallback](./iothub-client-core-h/iothubclientcore-setconnectionstatuscallback.md)            | 
[IoTHubClientCore_SetRetryPolicy](./iothub-client-core-h/iothubclientcore-setretrypolicy.md)            | 
[IoTHubClientCore_GetRetryPolicy](./iothub-client-core-h/iothubclientcore-getretrypolicy.md)            | 
[IoTHubClientCore_GetLastMessageReceiveTime](./iothub-client-core-h/iothubclientcore-getlastmessagereceivetime.md)            | 
[IoTHubClientCore_SetOption](./iothub-client-core-h/iothubclientcore-setoption.md)            | 
[IoTHubClientCore_SetDeviceTwinCallback](./iothub-client-core-h/iothubclientcore-setdevicetwincallback.md)            | 
[IoTHubClientCore_SendReportedState](./iothub-client-core-h/iothubclientcore-sendreportedstate.md)            | 
[IoTHubClientCore_SetDeviceMethodCallback](./iothub-client-core-h/iothubclientcore-setdevicemethodcallback.md)            | 
[IoTHubClientCore_SetDeviceMethodCallback_Ex](./iothub-client-core-h/iothubclientcore-setdevicemethodcallback-ex.md)            | 
[IoTHubClientCore_DeviceMethodResponse](./iothub-client-core-h/iothubclientcore-devicemethodresponse.md)            | 
[IoTHubClientCore_UploadToBlobAsync](./iothub-client-core-h/iothubclientcore-uploadtoblobasync.md)            | 
[IoTHubClientCore_UploadMultipleBlocksToBlobAsync](./iothub-client-core-h/iothubclientcore-uploadmultipleblockstoblobasync.md)            | 
[IoTHubClientCore_SendEventToOutputAsync](./iothub-client-core-h/iothubclientcore-sendeventtooutputasync.md)            | 
[IoTHubClientCore_SetInputMessageCallback](./iothub-client-core-h/iothubclientcore-setinputmessagecallback.md)            | 

## Macro definitions

#### IOTHUB_CLIENT_CORE_INSTANCE_TYPE

```C
#define IOTHUB_CLIENT_CORE_INSTANCE_TYPE
```

## Type definitions

#### IOTHUB_CLIENT_CORE_HANDLE

```C
typedef struct IOTHUB_CLIENT_CORE_INSTANCE_TAG* IOTHUB_CLIENT_CORE_HANDLE;
```

