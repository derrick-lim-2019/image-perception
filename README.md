# How to run application

## Important notes:
- Application was developed using a Linux Distribution (Ubuntu) with a CUDA-enabled GPU, and 
inference mode is run using a GPU.
- Mobile Application is built only for Android devices
- Both the server application & mobile application needs to be run on the same network.

## Server setup
1. Download weights to be used with application from this google drive link
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



 
