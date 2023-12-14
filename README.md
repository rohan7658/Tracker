A simple cybersecurity program to display network lines on google maps using python,wireshark and kml file Downloading external material: Python 3 which can be downloaded from the official Python webpage: https://www.python.org/ , Wireshark. This file contains a demo PCAP file which can be used. Capture Network Traffic: With Wireshark installed it’s time to create our input data which will consist of a captured pcap file. The file will consist of all network traffic going to and from our device in the period we have the capture function activated. Running the Code: When the code is executed ,copy the output to a file and save it with .kml to use it on google maps Adding Data to Google Maps: With our newly created .kml file, we’re now ready to add it to Google Maps. Navigate to https://www.google.com/mymaps. Here you can create a new map and Import a new layer.

For input data we are going to use Wireshark!

To initialize a capture open wireshark and select a interface which has traffic going through it.

When selecting a interface, Wireshark automatically starts a new capture, which is why you immediately gets prompted with network traffic. 

Once the capture has been stopped you need to export the captured data in pcap format, this can be done by clicking File -> Export Specified Packets.. and then selecting the following format: 

Wireshark/  -pcapng(*.ntar.gz;*.ntar.zst;*.ntar.lz4;*.ntar;*pcapng.gz;*pcapng.zst;*pcapng.lz4;*pcapng;)

With the captured data saved in the correct format, you’re ready to move into the Python Implementation.

A sample output for this would be 

![Screenshot (5)](https://github.com/rohan7658/Tracker/assets/117381038/bf31b427-4acb-4fdb-9d22-e6418555ce85)

