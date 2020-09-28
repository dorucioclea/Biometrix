# Biometrix: Artificial Intelligence Assisted Biometric Signature on Blockchain

Biometrix is a mobile application for signing any document in accustomed way with a state of the art level of security.  Principally Biometrix focusses on provide to a system for companies from all industries, banks, hospitals, government offices and other many organizations. The application focuses on dynamic (online) signature recognition which will be assisted by artificial intelligence for obviate forgeries and forensics. 

The importance of user authentication is a very important aspect especially when the number of users plus the size of the data to be checked against forgery has been increasing exponentially. Biometric Authentication can be done in many ways such as retina, voice, palm, or finger-print recognition. Along with those, the behavioral biometric verification can be used very effectively. A biometric signature is a behavioral biometric recognition that can be done by your actual handwriting signature on -say- a PDA using a digital pen. Biometric recognition systems have produced mostly for the reasons for Identification and Verification. Developing those systems for monitoring and providing access control is now a common practice in a variety of companies, banks, hospitals as well as in public organizations. We intend to develop a mobile application that provides signature verification and transaction management for documents that are hand-signed by clients. Since we deal with the biometric data of the users of the aforementioned organizations, surely the most important issue is security.

## Overview
For a long time signature has always been associated with that of law requirement. The usage of a signature confirms the identity of every individual. It creates a legally binding contract or agreement between two or more parties. Biometrix is a mobile application for signing any document with users biometric signature. Principally, Biometrix will provide conformity for companies from all industries, banks, hospitals, government offices, and other organizations.
Biometrix is a mobile application for signing any document in an accustomed way with a state of the art level of security. Principally the application focuses on dynamic (online) signature recognition which will be assisted by artificial intelligence for obviating forgeries.
Biometrix aims to solve another vital problem on our planet: tree
consumption for paper. With start to using Biometrix by both public and private
corporations, we may save billions of trees every year.

## Biometric Signature
The most significant benefit of signature recognition is that is highly resistant to impostors. After the user puts own signature on a mobile device, Biometrix captures dynamic pieces of information.This information consists of x-y coordinates, pressure, velocity, acceleration, time difference, pen tip force, azimuth, elevation angle of the pen and rotation about the pen axis.
In the capturing phase, we normalized location of the signature and removed the jagged of signature. Before we start to capture a signature, the signer could start to sign any location of the surface thus we normalized all x and y locations for each point. The tablet device may have a low resolution. So smoothing signature is an important preprocessing operation before extracting local features. Since signature data already collected from mobile device, we have to extract local features. After extraction, we will have 20 features for each point using for signature recognition:

![capture](https://github.com/taylanakbas/Biometrix/blob/master/Signature%20point.png?raw=true)

## Dynamic Time Warping
My chosen Artificial Intelligence Methodology for this project is Dynamic Time Warping” and, here how we deal with it.
The Dynamic Time warping algorithm is used to compare the similarity or distance between two time series with different length. It originates from the field of sound pattern recognition. Actually it can be used any temporal sequences of video, audio, graphics data or any data that can be turned into a linear sequence. Following figures demonstrates instance of two different test signature comparisons using with DTW.

![dtw](https://github.com/taylanakbas/Biometrix/blob/master/DTW.jpeg?raw=true)

## Blockchain
When a new user model created, the API generates a custom structure that consists of model data. Then it creates a new block and adds to our blockchain structure. This application is proof of concept so any decentralization operation has not placed here. The following representation shows how to store each data in our blockchain. Each block includes block information and client data. Biometrix stores client id, client's threshold and 5 different signature. Each signature consists of different number of point and for each point all local features are extracted and normalized.

## Transaction
After signing document, user confirms the process. Every confirmed signature defined as transaction. Transaction files are registered on the server. Each transaction file includes several  different type of files:

![capture](https://github.com/taylanakbas/Biometrix/blob/master/Transaction.png?raw=true)

Each file data captured by the mobile app and saved before transaction confirmed.

Following poster demonstrates structure of the project:

![capture](https://github.com/taylanakbas/Biometrix/blob/master/Architecture.png?raw=true)

---

**NOTE**

* You can find test result files of the software: [Sample](https://github.com/taylanakbas/Biometrix/tree/master/sample). This includes a signature model with geniue & forgery tests.
* You can also find the presentation of project here : [Presentation](https://github.com/taylanakbas/Biometrix/blob/master/Presentation.pdf)

---



