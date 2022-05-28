# 168



 create a basic web based AR app using pattern markers.
---------------------------------------


Hiro markers to display content over that, which is a standard marker.


create our own marker like we created image trackers.


EX:
start designing the AR content for the hotel menu card.

What if you can actually see the food ingredients and how the food will look in AR?

To display the food and its ingredients in AR, we are going to use our own markers. These are called pattern markers.
------------------------------------------------------------
SOLUTION:

Now, to create pattern markers we can take an image and create the pattern marker of that.

There are a few points that we need to keep in mind while creating pattern markers:

● It would be better if we use small size images to create markers.

 The markers should be in square shape.
● The black and grey colors are to be used as the background color of the marker.
● It's better to avoid transparent, white and any other colored background.
-----------------------------------------------------------

let's get started. We have the pizza image, and we are going to use it to create the pattern marker.


we are going to use another AR.js marker creating tool.
https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html


Once the image is uploaded we can set:
● Pattern ratio: this sets the size of the image with respect to the borders.
● Image size: size of the image.
● Background border color: set
to black color.
Click on the download marker and download image.
The marker will be downloaded in the .patt file format.

And the new marker image will be downloaded which we can use to detect AR content.

--------------------------------------------------------------
 let’s quickly add the pizza model asset using <a-assets>.
  
  <a-assets>
   <a-assset-item id= "" src="....scene.gltf" ></a-asset-item>
    
    </a-assets>
  
  -------------------------------------------------------
  
  tell the computer to identify the pattern marker.
  
  <a-marker> 

    id=""
type: “pattern”
url: file path to pattern maker descriptor (including .patt file extension) created before.
    ---
    </a-marker>
-----------------------------------------------------
  
  display the content of the marker
  
  add the content as the child of the <a-marker>.
  
  we can set the model and dish name with a list of ingredients in the dish.
We can use <a-plane> to display the text entities over the plane.
  
  
  
  As an extra feature for the pizza model, we can use the gesture-handler component, which is a part of this library, to rotate and scale up/down the model. (Make sure the gesture-detector component is attached to the <a-scene>.)

  ----------------------------
  
  
To see the output:
● Use ngrok to run the
application.
● Open HTTPS URL in your smartphone/laptop and give permission to use the camera.
● Open the marker image that was downloaded from the tool and point the camera towards it.
  
  Make the rotation mode is off while using the phone in landscape mode.
  
  *************************************************
 now  create the pattern marker and display content over that.
You will also add two buttons to allow the user to place orders and give ratings.
  
  
  add buttons to allow the user to order and rate the project.
We can add the <div> tag and write a component to add the button elements.

  
  create a .css file and add the styling to the button element.
Note 1: We are using the Bootstrap CSS library to style the buttons.
Note 2: Add the src to the index.html
  
  
  
  
  
