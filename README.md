- 👋 Hi, I’m @BrianBarakaKasamba
- 👀 I’m interested in cyber security and here is my simple implementation  to take a file of network traffic and convert it into a visual presentation using Google Maps.
- 👀Resources and applications is needed to make it work; WireShark , Python3 ,GeoLiteCity database as this will be used to translate a IP address into a Geo location(longitude & latitude). The database can be downloaded here: 
- https://github.com/mbcc2006/GeoLiteCity-data
- 👀Wireshark application to be able to capture network traffic on your device.
-  The Wireshark application can be downloaded here: https://www.wireshark.org/ The basics of Wireshark is out of scope for this test.
-  
**Capture Network Traffic**__
With Wireshark installed it’s time to create our input data which will consist of a captured pcap file. 
The file will consist of all network traffic going to and from our device in the period we have the capture function activated.
To initialize a capture open wireshark and select a interface which has traffic going through it. e.g
![wireshark2](https://user-images.githubusercontent.com/98221277/197357732-de57304c-f536-4eed-a3d7-694e66b52ad7.png)


Python Implementation
First off you will need to import the needed libraries, these are as follows:

import dpkt  --> is a python module for fast, simple packet parsing, with definitions for the basic TCP/IP protocols.
import socket--> socket module provides various objects, constants, functions and related exceptions for building full-fledged network applications including client and server programs. 
import pygeoip --> to corelate IP address with physical location.

Terms ;
KML - 
KML is a file format used to display geographic data in an Earth browser such as Google Earth. 
You can create KML files to pinpoint locations, add image overlays, and expose rich data in new ways. 

pcap - 
Packet Capture or PCAP (also known as libpcap) is an application programming interface (API) that captures live network packet data from OSI model Layers 2-7. 
Network analyzers like Wireshark create . pcap files to collect and record packet data from a network.

Python script to generate kml file compatible with google maps.
Will 
![proofgif](https://user-images.githubusercontent.com/98221277/197357961-dfce0e57-d445-49da-9bba-fa17cb96b2ca.gif)

Detailed report will be released soon.
Importing KML file to googlemaps
1.Naviget to https://www.google.com/maps/d/?hl=en
2.Create new map
3.Import KML file
![gmaps1](https://user-images.githubusercontent.com/98221277/197358105-911e6831-af24-4559-b59d-c608489c1119.png)
4.Open KML file and interact
![outcome](https://user-images.githubusercontent.com/98221277/197358505-8203151a-d374-45df-8ede-e8d29f5966e9.png)

