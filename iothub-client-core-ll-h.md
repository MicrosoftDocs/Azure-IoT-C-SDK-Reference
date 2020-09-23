---                             
title: "iothub_client_core_ll.h header file reference | Microsoft Docs" 
titleSuffix: "Azure IoT C SDK"            
description: "This is the header file reference page for iothub_client_core_ll.h in the Azure IoT C SDK. This SDK is used with Azure IoT Hub and Azure IoT Hub Device Provisioning Service"            
manager: timlt                 
author: wesmc7777              
ms.author: wesmc               
ms.date: 10/24/2018                    
ms.service: "iot-hub"             
ms.custom: ""                
ms.topic: "reference"        
---                            

# iothub_client_core_ll.h 

Internal APIs used by the Azure IoT C SDK to communicate with an Azure IoTHub.

Direct use of this library header is not supported.

## Includes

\#include <time.h>  
\#include "[azure_c_shared_utility/umock_c_prod.h](umock-c-prod-h.md)"  
\#include "[iothub_transport_ll.h](iothub-transport-ll-h.md)"  
\#include "[iothub_client_core_common.h](iothub-client-core-common-h.md)"  

## Detailed Description

IoTHubClientCore_LL is a module that allows a user (usually a device) to communicate with an Azure IoTHub. It can send events and receive messages. At any given moment in time there can only be at most 1 message callback function.

This API surface contains a set of APIs that allows the user to interact with the lower layer portion of the IoTHubClient. These APIs contain _LL_ in their name, but retain the same functionality like the IoTHubClient_... APIs, with one difference. If the _LL_ APIs are used then the user is responsible for scheduling when the actual work done by the IoTHubClient happens (when the data is sent/received on/from the wire). This is useful for constrained devices where spinning a separate thread is often not desired.

## Functions

Function Name                  | Description                                
--------------------------------|---------------------------------------------
[IoTHubClientCore_LL_CreateFromConnectionString](./iothub-client-core-ll-h/iothubclientcore-ll-createfromconnectionstring.md)            | 
[IoTHubClientCore_LL_Create](./iothub-client-core-ll-h/iothubclientcore-ll-create.md)            | 
[IoTHubClientCore_LL_CreateWithTransport](./iothub-client-core-ll-h/iothubclientcore-ll-createwithtransport.md)            | 
[IoTHubClientCore_LL_CreateFromDeviceAuth](./iothub-client-core-ll-h/iothubclientcore-ll-createfromdeviceauth.md)            | 
[IoTHubClientCore_LL_Destroy](./iothub-client-core-ll-h/iothubclientcore-ll-destroy.md)            | 
[IoTHubClientCore_LL_SendEventAsync](./iothub-client-core-ll-h/iothubclientcore-ll-sendeventasync.md)            | 
[IoTHubClientCore_LL_GetSendStatus](./iothub-client-core-ll-h/iothubclientcore-ll-getsendstatus.md)            | 
[IoTHubClientCore_LL_SetMessageCallback](./iothub-client-core-ll-h/iothubclientcore-ll-setmessagecallback.md)            | 
[IoTHubClientCore_LL_SetConnectionStatusCallback](./iothub-client-core-ll-h/iothubclientcore-ll-setconnectionstatuscallback.md)            | 
[IoTHubClientCore_LL_SetRetryPolicy](./iothub-client-core-ll-h/iothubclientcore-ll-setretrypolicy.md)            | 
[IoTHubClientCore_LL_GetRetryPolicy](./iothub-client-core-ll-h/iothubclientcore-ll-getretrypolicy.md)            | 
[IoTHubClientCore_LL_GetLastMessageReceiveTime](./iothub-client-core-ll-h/iothubclientcore-ll-getlastmessagereceivetime.md)            | 
[IoTHubClientCore_LL_DoWork](./iothub-client-core-ll-h/iothubclientcore-ll-dowork.md)            | 
[IoTHubClientCore_LL_SetOption](./iothub-client-core-ll-h/iothubclientcore-ll-setoption.md)            | 
[IoTHubClientCore_LL_SetDeviceTwinCallback](./iothub-client-core-ll-h/iothubclientcore-ll-setdevicetwincallback.md)            | 
[IoTHubClientCore_LL_SendReportedState](./iothub-client-core-ll-h/iothubclientcore-ll-sendreportedstate.md)            | 
[IoTHubClientCore_LL_SetDeviceMethodCallback](./iothub-client-core-ll-h/iothubclientcore-ll-setdevicemethodcallback.md)            | 
[IoTHubClientCore_LL_SetDeviceMethodCallback_Ex](./iothub-client-core-ll-h/iothubclientcore-ll-setdevicemethodcallback-ex.md)            | 
[IoTHubClientCore_LL_DeviceMethodResponse](./iothub-client-core-ll-h/iothubclientcore-ll-devicemethodresponse.md)            | 
[IoTHubClientCore_LL_SendEventToOutputAsync](./iothub-client-core-ll-h/iothubclientcore-ll-sendeventtooutputasync.md)            | 
[IoTHubClientCore_LL_SetInputMessageCallback](./iothub-client-core-ll-h/iothubclientcore-ll-setinputmessagecallback.md)            | 
[IoTHubClientCore_LL_UploadToBlob](./iothub-client-core-ll-h/iothubclientcore-ll-uploadtoblob.md)            | 
[IoTHubClientCore_LL_UploadMultipleBlocksToBlob](./iothub-client-core-ll-h/iothubclientcore-ll-uploadmultipleblockstoblob.md)            | 
[IoTHubClientCore_LL_UploadMultipleBlocksToBlobEx](./iothub-client-core-ll-h/iothubclientcore-ll-uploadmultipleblockstoblobex.md)            | 

## Type definitions

#### IOTHUB_CLIENT_CORE_LL_HANDLE

```C
typedef struct IOTHUB_CLIENT_CORE_LL_HANDLE_DATA_TAG* IOTHUB_CLIENT_CORE_LL_HANDLE;
```

