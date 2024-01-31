BROADCAST RECEIVERS IN ANDROID APP DEVELOPMENT 

Receviers are broadcast messages that are sent when an event of interest occurs 

example; system boots, Device starts charging, when the charge of device is low and etc

When a broadcast message is sent , the system atomatically routes broadcasts to apps that have subscribed to receive that particular type of broadcast

we use receivers to sent broadcast messages in our app for stuff such as low battery, wifi connectivity , airplane mode , or other runtime processes which needs an app subscription. 

e.g. a photo upload app liek Google drvie will prefer to use wifi to upload photos to reduce mobile data usage. A receiver will be adequate to check when the device connects to a wifi , and when the system event notifies that the device is connected to wifi, the photos can be uploaded to the server. 

- Braodcast messages to receivers can be sent between two applications , or an application and the system OS application. 

two methods to define the broadcast receiver: 

-through the android manifest file 
- the context registered method class 

NB: For Android Oreo(API 26) and later, you must create the "Broadcast recevier" from Java class, not from Manifest file. Since our first example in this project is about creating a "Broadcast receiver" from the Manifest file, you should test it with API 25 and earlier. Otherwise you cannot create a "Boradcast Receiver". For API 26 and later, we will create "BroadCast Receiver" over java class in our second example in this video.  

