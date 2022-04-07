# How to run application

## Important notes:
- This is Group 3's implementation of the Supermarket Group Project for CS424 Image Perception
- This implementation involves a hosting server and an application
- Application was developed using a Linux Distribution (Ubuntu) with a CUDA-enabled GPU, and 
inference mode is run using a GPU.
- Mobile Application is built only for Android devices
- Both the server application & mobile application needs to be run on the same network.

## Server setup
0. Download code file (Cannot fit on github here) from this link
https://drive.google.com/file/d/14kBKJAuWUc3g1hQlV-DVfATaTOv9ZaLb/view?usp=sharing
2. Download weights to be used with application from this google drive link
https://drive.google.com/file/d/1rLzAXHdn6lGZ3XKHaW5oMC9atPffmVvj/view?usp=sharing
2. Open ```app.py``` and change line #14 to the path of the downloaded weights
3. Change directory to the root of the downloaded folder and you should see a ```requirements.txt``` file, run the following command in the terminal ```pip install -r requirements.txt``` to install dependencies for the application
4. Change the directory by running ```cd darknet``` and you should see the file ```app.py```
5. Run the application with ```python app.py```
6. Your server should now be running on all addresses of the network on port 5000.

## Mobile Application setup
1. Download Android application from this google drive link
https://drive.google.com/file/d/1u1SyAicePfmBEUYBN2vvhfUrIvKduZRQ/view?usp=sharing
2. Install application on your mobile phone
3. Find out the ipaddress of your server and replace the server url in the application
4. Your mobile application should be ready to be used with the inference server

## How to use
1. Visit the hosted server's URL at ```http://{ip_address}:5000/images``` on your browser to reach a landing page. Ensure that the device's browser is within the same network.  

![Browser Page View](https://github.com/derrick-lim-2019/image-perception/blob/59cd145c8b049f9ac201847ee0a11127287166f8/images/Browser%20Landing.JPG)

3. Launch the mobile application and enter the hosted server's URL at ```http://{ip_address}:5000``` as a target  

![Mobile App View](https://github.com/derrick-lim-2019/image-perception/blob/59cd145c8b049f9ac201847ee0a11127287166f8/images/photo_2022-04-07_13-54-19.jpg)

4. Choose a photo from your gallery / take a new photo and hit "Predict Class". 

![Mobile App View 2](https://github.com/derrick-lim-2019/image-perception/blob/59cd145c8b049f9ac201847ee0a11127287166f8/images/photo_2022-04-07_13-54-17.jpg)


5. Receive response on both your Android device and your browser  

![Mobile App View 3 ](https://github.com/derrick-lim-2019/image-perception/blob/59cd145c8b049f9ac201847ee0a11127287166f8/images/photo_2022-04-07_13-54-11.jpg)

![Browser View 2](https://github.com/derrick-lim-2019/image-perception/blob/59cd145c8b049f9ac201847ee0a11127287166f8/images/Detection.JPG)
 
