# ML_Based_Smart_Watch
Machine Learning and Microcontroller based smart watch
# Smart-Watch-Design
In this project, to design a smart wristwatch that has the capability of geographic positioning as well as measuring the heart rate of the person under care, as well as processing the data related to the heart rate sensor and processing the deep recursive network on this data and detecting the current state of the person, i.e. "The person has fallen" or "The person is trapped" or "The person is alive or dead" and finally "The person is injured". To achieve this, the Sisfall dataset and also the detection of the falling situation with the help of Recurrent Deep Neural Network (RNN) and finally putting the trained model on the esp32-wroom32 microcontroller and processing the real data received from the pulse sensor and sending the output result to the server environment which in this project is from Google Sheet for Display and storage of data related to the location, as well as data related to the heart rate sensor and data related to the output of the trained model (one of the 5 types of activities related to daily activities and falling), are used In this project, in order to detect whether a person is trapped or alive or dead or injured, by using the heart rate sensor data that can be seen in the Google Sheet environment, these situations can be In order to diagnose the condition of a person being wounded, this condition can be understood from the decrease in the heart rate, or in a period of time when the location of the person does not change and the heart rate is increasing, this possibility can be given. that the person is confined in this location, and if the heart rate becomes zero, it means that the person has cardiac asystole and is dead. In this project, low-power modules are used, which increases The life of the battery and the power supply of the device is consumed. Therefore, in this project, 3.7 V 1000 mAh battery modules are used to power the device, Ublox Neo6M GPS module is used to determine the geographic location, and the pulse sensor module is used as above. It was mentioned, it was used to determine the heart rate of the person under care.
The link related to this project is given below and it should be mentioned that Python language was used to design the recurrent deep neural network (RNN) and Arduino programming language was used to code the esp32-wroom32 microcontroller, in the not too distant future it will be possible to detect The four mentioned situations are possible with the help of artificial intelligence.
# Circuit Schematic:
"The circuit schematic of the smart wristband is as illustrated in the provided schematic diagram file.This circuit uses the ESP32-WROOM-32 module and a tester circuit to achieve extended flash memory (4MB) for saving the model. It processes real data received from sensors, such as a pulse sensor, feeds this data to the model, and outputs the results. This setup aims to achieve a more reliable and high-scoring model for activity detection.
# Code Explanation:
Initially, I installed the required libraries using pip install, specifically the swarm library for the Particle Swarm Optimization (PSO) algorithm, and the everywhereml library for converting Python code to MicroPython or Arduino code. In the Colab environment, since other libraries are pre-installed, it was only necessary to import them. The numpy library was used for algebraic computations, such as vector and matrix definitions and inner product calculations. The sklearn library was employed for implementing machine learning algorithms, particularly the Random Forest algorithm in this project. It was also used for measuring model parameters and splitting the dataset into specified ratios for training and testing.Subsequently, the parameters for the machine learning model and the PSO optimization algorithm were defined. The resulting model was then converted into Arduino code, allowing it to be executed on a microcontroller, specifically the ESP32-WROOM32 used in this project. For further information, please refer to the links below.

for learn more about machine learning algorithm with python,Please refer to the reference below.

https://maktabkhooneh.org/course/%DB%8C%D8%A7%D8%AF%DA%AF%DB%8C%D8%B1%DB%8C-%D9%85%D8%A7%D8%B4%DB%8C%D9%86-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86-mk1318/

for learn more about metahuristic algorithm with python,Please refer to the reference below.

https://biglearn.ir/product/%D8%A2%D9%85%D9%88%D8%B2%D8%B4-%DA%A9%D8%A7%D9%85%D9%84-%D8%A7%D9%84%DA%AF%D9%88%D8%B1%DB%8C%D8%AA%D9%85-%D9%87%D8%A7%DB%8C-%D9%81%D8%B1%D8%A7%D8%A7%D8%A8%D8%AA%DA%A9%D8%A7%D8%B1%DB%8C-%D8%A8%D8%A7/

In the Arduino code, the WiFi library is used to connect the ESP32-WROOM-32 module to a router for internet access. The HTTP Client library is used to connect to the server, which in this project is Google Sheets. The TinyGPS++ library configures the NEO-6M GPS module to communicate with GPS satellites and determine geographic coordinates (latitude and longitude). The hardwareserial library enables communication between the modules and sensors using the specific protocol with the ESP32-WROOM-32 module. The communication protocol between the ESP32-WROOM-32 module and the GPS module is UART. The code defines the machine learning model as a class, and it includes steps for receiving data from sensors, connecting to the router, sending data to Google Sheets, storing the data, and displaying the data in Google Sheets.

# Dataset

In this project, the SisFall dataset is used for detecting falls and other activities. The reason for using this dataset is its good flexibility and because, in this project, we used a pulse sensor module to detect activities. By using this dataset, this can be achieved.The Google Drive link for the dataset of this project is as follows:

https://drive.google.com/file/d/1aKhckbgBz7y0fD_01hVQfL6fBFLHmb3s/view?usp=drive_link

# How the Project Works

To Execute:

1.Open the Python file with Google Colab.

2.It doesn’t matter whether you want to run the project with a GPU, TPU, or CPU.

3.Use the mount Google Drive capability to connect Google Colab to Google Drive by navigating to the project folder in the Telecommunications Networks course, whose link is provided at the end of the README.

4.Place the directory address of sisfall.csv in the directory path within the Python code.

5.Copy the Arduino code generated by Python to the location under libraries in the Arduino file.

6.Upload the Arduino code to the ESP32-WROOM32 module using the Arduino IDE.

7.Congratulations. The project is now executable.

Google Drive link,description of the smart wristband design project:

https://drive.google.com/file/d/1uN2HTS5Wt-oqSwqVQp-O_pPVzVAf4x2C/view?usp=drive_link

Google Drive link of the project and all class activities:

https://drive.google.com/drive/folders/1t60cGLn013Ep5F4Ft_9nn4Ba7i-FDGYs?usp=drive_link

my email address:

mohammadreza.dolatshahi.76@gmail.com

Telegram ID:

@ Mohammadreza_Di5

ORCID Number:0009-0008-2612-6046
