# Halusky detector
In this project you have all the required files and links in order to train [Watson Visual Recognition](https://console.bluemix.net/catalog/services/visual-recognition) to recognize [Halusky](https://en.wikipedia.org/wiki/Halu%C5%A1ky)
In the folders above you can see examples of halusky and sets of examples of items which can be mistakenly categorized as halusky, hence 
with the negative examples you can point Watson Visual recognition to the correct set of features for real halusky. 

## How to create your own visual recognition for Halusky
1. Get and account in [IBM Cloud](https://ibm.com/cloud)
2. Setup istance of [Watson Visual Recognition](https://console.bluemix.net/catalog/services/visual-recognition) service
3. Create a class for [Halusky](https://en.wikipedia.org/wiki/Halu%C5%A1ky) 
    1. As you can see in the dashboard there's already a "NotClass" provided for you 
4. Attach uploaded files to respective classes (Halusky to halusky class, anything else to NotClass)
5. Start the training by clicking "Train" button 
6. After some time you will have a class trained to recognize halusky.

Now you can utilize REST endpoint or CoreML to use your trained class. 

## What we did with Telegram 
Requirements: 
1. [Telegram](https://telegram.org) account 
2. [IBM Cloud](https://ibm.com/cloud) account 
3. [Node-red](https://console.bluemix.net/catalog/starters/node-red-starter) instance
4. Telegram nodes for node-red 

In the files of this repository you can find also a flow designed to utilize your trained class and a Telegram bot 
which you can create via talking to [BotFather](https://telegram.me/BotFather) in Telegram platform. 

## Watson visual recognition service 
As you can see in the visual recognition service all you need to start a class is 10 pictures, please do keep in mind that the number of example (positive & negative) images is important as training events count towards your API usage which with lite plan is limited. 

[The Flow.json](./telegram-node-red-flow.json)
