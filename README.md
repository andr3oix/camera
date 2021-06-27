# Camera
This project is used to demonstrate how easy a web app can use your camera to take a photo. As long as you give permissin to this web app to use your camera when you launched the page, it can take your camera photo right away without any further notification. 
- on the mobile devices, phone or tablet, it will use front camera to take the photo.
- https connection will be required for most of browsers. Using http, most browsers will not be able to get Camera permission.

Try this app using Heroku.[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?template=https://github.com/51sec/camera/master)

Once you visited this page, it will ask your camera permission then automatically take a photo from your camera without any further step. 


# Screenshots
![alt text](https://photos.51sec.org/file/test1-51sec/2021/06/msedge_tCD3zF5PIW.png)

Captured Photo will be placed into website /photos/ folder

- https://camera51.herokuapp.com/ : It will ask your permission to use camera then take a photo from your camera automatically. The phone taken by camera will be saved into the folder named by your public ip. 

Note: The photo will be deleted automatically once Heroku app is in idle. It will be active 12 hours/day from 8AM - 8PM. 


To manage the camera photo, you might need to use another php script to view/delete/upload your photos. 
- In this project, I integrated the one from https://github.com/jcampbell1/simple-file-manager .
The code has been put into index.php file under photos folder to make the whole project easy to use.

- https://camera51.herokuapp.com/photos : simple file manager to manage your photos. You can view or delete the photos taken by this app. 


Notes:
Original index.php and photo.php code is from SunPma's blog post,“https://sunpma.com/994.html”. I tanslated all to English and add simple-file-manager code into it. All codes are belongs to original authors. 
