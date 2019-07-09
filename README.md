# Fire Alarm using Watson Visual Recognition

This project is a how-to guide on using Watson Visual Recognition service to analyse an image and based on a trigger word then send a event command to IoT Device.In this example node-red is used to create an image upload form which sends the image to Watson Visual Recognition and trigger an iot device whenever fire is detected in the image.

 # NOTE: Please check the Video tutorial at the bottom if you have issues.

1. Login/signup in to your [IBM Cloud Account](https://ibm.biz/BdYtcs)
2. Goto Catalog and create the following services:
* [Internet of things Platform starter](https://console.bluemix.net/catalog/starters/internet-of-things-platform-starter)
NOTE : You need to create the A Platform Starter App,not Internet of things Platform service.I suggest you use the link above to quickly avoid confusion.
* [Visual Recognition](https://console.bluemix.net/catalog/services/visual-recognition)

![creating Services](https://github.com/krishnac7/Media/blob/master/IotImageAnalysis/Gif/creatingServices.gif)

NOTE: You can skip steps 3,4 & 9

3. Goto connections tab and open IotF Service and Launch Watson Iot Platform
4. Navigate to Devices tab and Add Device

![Adding devices](https://github.com/krishnac7/Media/blob/master/IotImageAnalysis/Gif/creatingDevice.gif)

5. Once the Starter app is running,visit app url and configure Node-red
6. Login to your node-red flows dashboard and import flow from [flows.json](https://github.com/krishnac7/IotImageAnalysis/blob/master/flows.json)

![Importing Flows](https://github.com/krishnac7/Media/blob/master/IotImageAnalysis/Gif/importing%20Flows.gif)

7. Create new visual recognition credentials

![Create visual recognition credentials](https://github.com/krishnac7/Media/blob/master/IotImageAnalysis/Gif/VisualRecognitionServiceCredentials.gif)

8. Update api key in the visual recognition node-red flow
9. Update the device details in IBM Iot device node {Optional}

![Updating credentials](https://github.com/krishnac7/Media/blob/master/IotImageAnalysis/Gif/updateCredentials.gif)

10. Visit <app_url>/upload and upload required image
11. Change the string inside includes from trigger action function to set a different trigger


[Video Tutorial](https://github.com/krishnac7/Media/blob/master/IotImageAnalysis/imageAnalysisIot.mp4)
