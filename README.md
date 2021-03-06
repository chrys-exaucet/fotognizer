# Recognito

## Purpose
  A real time face recognition and authentication application,
with additional image processing in a user's gallery.
        
## Prerequisites
  - *MatlabR2020a* or higher
  - *App Designer*
  - Computer Vision Toolbox
  - Image Processing Toolbox
  - Statistics and Machine Learning Toolbox
  - Matlab Support Package for USB Webcams
  
  You can download and install necessary packages on Matlab Add-Ons site [here](https://www.mathworks.com/products/matlab/add-on-explorer.html).
  Follow the tutorial available on the *FaceApp-Demo folder* for furher informations.
 
## Technologies
1. _*Viola-Jones*_ algorithm for face detection. More about it [here](https://en.wikipedia.org/wiki/Viola%E2%80%93Jones_object_detection_framework).
2. _*Eigenfaces*_ for face recognition and tracking. More about it [here](https://en.wikipedia.org/wiki/Eigenface).
 You can still review the [Resourceful-Links.txt](Documentation/Resourceful-Links.txt) file for further intels.



## Application Structure
  The application opens on an authentication or registration interface by facial recognition.                                             
  An authenticated user can apply a set of operations on an image in his database, via his personal space; those are: load, filter, rotate, reset or save changes.

##  Files
  The initial login interface with embedded real time face recognition is on the [Connexion.mlapp ](src/Connexion.mlapp) file. 
  Follow the instructions given through the interface.
  Do register your face before trying to be recognized.


  [UserInterface.mlapp](src/UserInterface.mlapp) is the interface of the user's personal space. 
  Must be called by the first interface! Otherwise, comment the first 3 lines of its startupfcn.

  The [Database](Database) folder called inside the Connexion.mlapp to recognize regeistered faces. You can add there your set of faces, each in a signle folder.
  Note the the way you will name your folder inside the database is the name you should use to get registered with the app.

  If you move the database folder elsewhere or change its name, please modify the database private property inside the Connexion.mlapp accordingly.
                         
  [FaceApp-Demo](FaceApp-Demo/) contains demo videos and photos of the app installation, look&feel and behavior.
  You may look at it for convenience.

 [FaceAppLogo.jpg](assets/FaceAppLogo.jpg) is Logo of the  application, visible via the second interface. If you move the file elsewhere or change its name, please modify the logo private property inside the UserInterface.mlapp accordingly.

`Any trouble or insight? Feel free to open an issue`.
  
