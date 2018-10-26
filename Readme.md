#Halusky detector
In this project you have all the required files and links in order to train Watson Visual Recognition to recognize Halusky[]
In the folders above you can see examples of halusky and sets of examples of items which can be mistakenly categorized as halusky, hence 
with the negative examples you can point Watson Visual recognition to the correct set of features for real halusky. 

## How to create your own visual recognition for Halusky
1. get and account in IBM Cloud []
2. setup istance of Watson Visual Recognition service []
3. Create a class for Halusky 
    a. as you can see there's already a "Not" class provided for you 
4. attach uploaded files to respective classes (Halusky to halusky class, anything else to NotClass)
5. start the training by clicking "Train" button 
6. After some time you will have a class trained to recognize halusky.

Now you can utilize REST endpoint or CoreML to use your trained class. 

## What we did with Telegram 
Requirements: 
1. Telegram account 
2. IBM Cloud account 
3. Node-red instance 
4. Telegram nodes for node-red 

in the files of this repository you can find also a flow designed to utilize your trained class and a Telegram bot 
which you can create via talking to FatherBot in Telegram platform. 