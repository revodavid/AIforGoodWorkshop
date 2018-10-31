# AI for Good Workshop

## ODSC West, November 2018

The Seeing AI app (available on the iOS App Store) provides tools for blind and vision-impaired people to assist with everyday tasks. Many of the functions in the app are implemented with [Cognitive Services](https://azure.microsoft.com/en-us/services/cognitive-services/) in Azure.

In this workshop, we'll experiment with various [Cognitive Service APIs](https://azure.microsoft.com/en-us/services/cognitive-services/directory/vision/) used in the Seeing AI app to see how they behave and learn about the type of data they return. We will be using only the web demo interfaces, so you won't need an Azure subscription and you'll only need a web browser to try them out. 

The demo pages typically include sample data (photos, etc) you can try, but we encourage you to find your own data and see what happens. You can use a file on your laptop or the URL of a file of on the Web. Here are some things you can try:

* [Random Wikimedia page with an image](https://commons.wikimedia.org/w/index.php?title=Special:Random&prop=images). Click the download button to get a direct URL (often with a choice of resolutions).
* [ImageNet](http://www.image-net.org/). Type a word into the search box to find images by category.
* [Google Images](https://images.google.com/). It can be tricky to get a link to an image: click on a result and right-click on a large image (_not_ a thumbnail) to get a URL.
* Your own media files. Unless they are accessible by URL, you'll need to download them to your laptop first (in a suitable format/size)and use the "Browse" button on the demo page to upload them. Microsoft does not store media submitted on these pages.

No programming will be required in this part of the workshop. If you'd like to learn how to use Cognitive Services from application via the API or language SDKs, try this Microsoft Learn module: [Process images with the Computer Vision service](https://docs.microsoft.com/en-us/learn/modules/create-computer-vision-service-to-classify-images/index).

# Vision

In the Seeing AI app, the "Person" feature detects people in the camera frame in real time, and describes them when pressing the camera button. Try it in the app now.

* Click the "Person" button in the Seeing AI app
* Point the camera at a face; an audio guide will alert you when a face is in frame
* Tap the screen to get detailed information about the faces on the screen

## Face API

The [Face API](https://azure.microsoft.com/en-us/services/cognitive-services/face/#detection) will detect one or more human faces in an image, and return information about the location and attribute of those faces.

* Visit the [Face Detection](https://azure.microsoft.com/en-us/services/cognitive-services/face/#detection) page.
* Copy the URL of an image to the "Image URL" box, or click "Browse" to upload an image, then click Submit.
* Your image will be shown on the page with a rectangle bounding all detected faces.
* Look at the results in the right pane to see the detailed analysis. The JSON array will include one element for each detected face.
* The `faceRectangle` property defines the bounding box of the face(s).
* The `faceAttributes` propery includes details about the person's appearance, such as hair color/baldness, type of facial hair, presence of glasses and headwear, use of makeup, etc.
* The `faceAttributes` section also includes the person's apparent gender, age, and intensity of emotion (anger, happiness, surprise, etc) on a scale from 0-1.
* The `faceLandmarks` property locates specific parts of the face (pupils, tip of the nose, corner of the mouth, etc) within the image
* Check the [FACE API Reference](https://docs.microsoft.com/en-us/azure/cognitive-services/face/apireference) for other attributes that may be of interest.

Things to try: [Sikh man](https://commons.wikimedia.org/w/index.php?search=man&title=Special%3ASearch&profile=default&fulltext=1#/media/File:Sikh_man,_Agra_10.jpg), [Woman in comic store](https://upload.wikimedia.org/wikipedia/commons/e/e7/7.9.10OliviaMunnByLuigiNovi53.jpg), [woman performing at concert](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4a/We_Are_X%2C_post-screening_concert%2C_SXSW%2C_Austin%2C_Texas_2016-0531_%2843210344362%29.jpg/400px-We_Are_X%2C_post-screening_concert%2C_SXSW%2C_Austin%2C_Texas_2016-0531_%2843210344362%29.jpg).

# Documents

The Seeing AI app 

# Handwriting

The "Handwriting" tool in Seeing AI

[Handwriting Recognition](https://azure.microsoft.com/en-us/services/cognitive-services/computer-vision/#handwriting)

Things to try: [Analytics notepad](https://upload.wikimedia.org/wikipedia/commons/b/bd/Handwritten_Text.jpg),

# Custom Vision

Learn: https://docs.microsoft.com/en-us/learn/modules/classify-images-with-custom-vision-service/index




