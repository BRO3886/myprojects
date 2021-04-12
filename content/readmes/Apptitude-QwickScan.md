---
title: Apptitude-QwickScan
date: 2021-04-12T08:09:14+0000
draft: false
---
# Apptitude-QwickScan
>Submission for Apptitude 2020 by Team Behencode @BRO3886 @rithikjain

<div align="center">
<br>
<img src="https://raw.githubusercontent.com/BRO3886/qwickscan/master/screenshots/banner.png?token=AJQCPIWOA6QY4T3LH3CRENK7E3LYQ">
</div>

## The Idea

The idea for this app was very simple. We go to supermarkets and nearby grocery stores even during this pandemic because getting suppies for home is absolutely essential.

A problem we found with the system here in India is that even though people sometimes follow social distancing, but in long queues, lack of pateince gets the best of us. Thus, we rarely see people following social distancing on cash counters.

So we came up with this app (..or you could say 2 apps). 

We have 2 apps- 

Qwickscan Client side, Qwickscan admin side

The client (or the person whos' grocery shopping) can add scan the items and quick add it to their cart. 
This cart is synced with our servers

Whenever they reach the billing counter, they can show a QR and the entire bill comes to the admin.

Now, the admin can verify the items or just process it ahead for payment.

In this way we reduce the queues and reduce paper waste generated by those long bills.

Thank You.

## Features

**Client Side**

- [x]  Login/Sign Up
- [x]  Splash Screen (Hack Requirement)
- [x]  Create Cart
- [x]  Adding items to cart (via TfLite object detection)
- [x]  Displaying QR code of Cart (every cart has unique ID)

**Admin Side**

- [x]  Splash Screen (Hack Requirement)
- [x]  Scan QR Code of Cart
- [x]  Displaying items in scanned cart


We also thought about integrating payment options for checkout after confirmation from admin, but due to the limited time, we could not do.

## Link to the Repos

* [Client Side](https://github.com/BRO3886/qwickscan)
* [Admin App](https://github.com/rithikjain/qwikscan-admin-app)
* [Backend](https://github.com/rithikjain/qwikscan-backend)



## Instructions to run

* Pre-requisites:
	- Android Studio
	- Phyical Android device
    - Flutter
    - VS Code (recommended)

* Directions to install
```bash
git clone https://github.com/BRO3886/qwickscan
```

* < directions to execute >

```bash
cd qwickscan
flutter run
```



## Resources

[Design- Figma File](https://www.figma.com/file/GnB8hOq9JGvUX5EfHZV8fU/Apptitude?node-id=3%3A5)

[Drive Link for video and app](https://drive.google.com/drive/folders/1aqZCTdJY-sRg3sygGL9eyLCruzt0T50G?usp=sharing)

## Challenges Faced

* We were working for the first time with TFLite and real time object detection
* Had to figure out the appropriate UI on top of camera feed
* Laying out widgets on top of native views is difficult in Flutter.
* Luckily we found a way to do that.
* As a challenge, we tried implementing this with bloc. Considering the amount of boilerplate code needed for bloc,  I feel great about how quikly I can implement it now.

## Completion Status

Due to the time constraint, we could not complete the following:

* Payment integration with UPI to enable cashless transaction
* Implementing an inventory of items on the server
* Deleting items from cart (shit!)


## Learning and Key Takeaways

* We can make a backend in Go
* We can easily implement Bloc for state mangement
* Bloc is prolly the best solution for state management in fluter
* Flutter and TFlite is somewhat stable
* The best way to go ahead with implemting ML is through MLKit (lol)
* The app is performant, but bloated in size


Thanks a lot to [ACM-VIT](https://acmvit.in/) for giving us this opportunity!
