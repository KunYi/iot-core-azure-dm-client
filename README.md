# dm-proto-private

To build:

(1) Create a new folder and make it the current folder:
    md d:\Projects\AzureDM
    cd d:\Projects\AzureDM

(2) Enlist in the Azure SDK
    git clone --recursive --branch develop https://github.com/Azure/azure-iot-dt-sdks.git

(3) Build the Azure SDK
    pushd.
    cd azure-iot-dt-sdks\
    md cmake
    cd cmake
    cmake d:\Projects\AzureDM\azure-iot-dt-sdks\c
    Open d:\Projects\AzureDM\azure-iot-dt-sdks\cmake\azure_iot_sdks.sln
    Build:
        aziotsharedutil
        iothub_client
        iothub_client_mqtt_transport
        umqtt

(4) Enlist in the DM client
    git clone --recursive --branch master https://github.com/ms-iot/dm-proto-private.git

(5) Open d:\Projects\AzureDM\dm-proto-private\IoTDMAgent\IoTDMAgent.sln
    Build.