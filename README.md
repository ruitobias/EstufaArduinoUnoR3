# Smart Greenhouse
This is an IOT project which aims to track greenhouse status, in addition to "Automatic" &amp; "Manual" irrigation.


## Application
This application is made with ❤ by using "Flutter" framework, using "Bloc" architecture!
The application consists different pages to track sensors, irrigate manually and also set a threshold for automatic irrigation.


![Design](https://user-images.githubusercontent.com/36487462/88291030-e136fb80-cd0c-11ea-91bb-50e71eb7918a.jpg)


### How to use application
For help getting started with Flutter, checkout
[Flutter Documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
A few resources to get you started if this is your first Flutter project:
- [My online YouTube course (In Persian)](https://www.youtube.com/watch?v=gMvpTVj7joM&list=PLdSCNgAdv3IHaUmmwp__qvji8k-FyKvo3)
- [Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Useful Flutter samples](https://flutter.dev/docs/cookbook)


# Embedded Hardware Core
This project uses an "Arduino UNO" and "Wemos D1 mini" as hardware core.
Upcoming folders contain certain files & headers used for each microcontroller.
You can see schematics in following pictures:
### Note:
"Wemos D1 mini" connects to a router to access internet. Do not forget to set SSID & Password of your modem in following file:
"Embedded Hardware Core/wemos/wifi.h"


# Server
This project uses two servers to operate correctly.
- Local server is set to store sensor data as well as communicating with application.
- Telegram bot Server contains API for track & control hardware via "Telegram Application"

## Django Local Server:
This folder contains files for database and backend, using Python & Django framework.

![Server](https://user-images.githubusercontent.com/36487462/86034625-39514980-ba50-11ea-90ae-69be14098896.jpg)

### How to use local server
- Open terminal in mentioned folder
- type ".\venv\Scripts\activate" in CMD
- type "py manage.py runserver 192.168.1.102:8000" in CMD

Note: "192.168.1.102" is my laptop IP after connecting to router. You can access your own IP by running "ipconfig" in CMD.
Keep it in mind that all modules and also application are running on this local IP.

## Python Telegram Bot Server
This folder contains API for Telegram Bot, using Python.

![Telegram Bot](https://user-images.githubusercontent.com/36487462/88298932-029ce500-cd17-11ea-9668-be1ace7934ed.jpg)
