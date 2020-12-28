# Azure-IoT-Central-AZ3166-Setup

I bought an Microsoft Azure IoT capable <A HREF="https://en.mxchip.com/az3166"> MXChip AZ3166 </A> in early 2019, and when I got round to using it again with <A HREF="https://azure.microsoft.com/en-au/services/iot-central/">Azure IOT Central</A> in December 2020 I found that a lot of things had changed.

The origional purchase was inspired by <A href="https://www.hanselman.com/blog/did-i-leave-the-garage-door-open-a-nocode-project-with-azure-iot-central-and-the-mxchip-devkit" >Scott Hanselman's garage door opener</A>.

In order to get it working you need to get the latest devkit - https://github.com/Azure/iot-central-firmware . I used the 2.1.2 firmware <A HREF="https://github.com/Azure/iot-central-firmware/releases/tag/mxchip-v2.1.2"> here</A>.

Do note that the project above is marked as archive as of August 2020, so there are unlikely to be any new updates. I also tried the <A HREF="https://github.com/microsoft/devkit-sdk/releases/">IoT Hub page</A> firmware, but could not get the device to connect to IoT Hub at all. I suspect there is some infrastructure change in Azure preventing this.

The Microsoft Azure IOT Central still works as fine as before, however it no longer has a template for my device! I'm not sure why they removed it, so I have recreated from the raw data and am sharing here on Github.

Step 1: In your Azure IOT Central account, go to Device Templates and create 'New'


Step 2: Create a custom device template IOT 'Device'. Click 'Next: Customize':

Step 3: Give your template a name. Click 'Next: Review', then 'Create'.

Step 4: Click 'Import a model'. At this point select the AZ3166.json file I am sharing here.


That's it. You can now assign your device to this template.





