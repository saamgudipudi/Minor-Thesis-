
## Getting Started

Consider the mobile phones as sensors that sends constant readings to an edge device which runs the proposed BIRCH algorithm. At the edge, the data is checked for 
anomalies with the help of BIRCH algorithm. If the received reading is classified as an outlier than it is reported else it is sent to the server.


### Network 

Step by Step procedure: (Network)

Say what the step will be

Open source Tools:

ZeroTier : https://my.zerotier.com/network/a0cbf4b62a9f362f
Network ID: “a0cbf4b62a9f362f”

User Name : rahulg2526@gmail.com
Password: Deakincyber123

Can add upto 50 sensors, as soon as the new device is added to the network, they will be assigned to a virtual public IP. 

PRTG Monitoring Tool:  https://www.paessler.com/prtg 
PRTG server will run on local server http://127.0.0.0 on the local machine. 
Latency is calculated with ICMP monitoring sensors. 

External factors included in testing:

Based on this connectivity we had tested cloud architecture environment by sending multiple signals and different size of data from remote location to cloud. ( Just to add latency to any cloud server will never be constant it varies based on already existing traffic on ISP lines ), to make sure latency reports are legitimate readings are monitored in 1 minute interval with the help of open source monitoring tool PRTG, Where dark blue line in the reports indicates the average of all latency over one minute interval, where pink line indicates maximum latency obtained in that particular and  light blue line indicates minimum latency obtained in that one minute interval. 
Above all as it’s a real time testing what all external factors influence testing. 
1.	Latency is inversely proportional to bandwidth used in the line, i.e. if the bandwidth of the line is used to maximum extent the latency is more. If the bandwidth of the line used more than the actual capacity the latency will be higher than expected and can observe packet loss. 

2.	Size of the data is directly proportional to bandwidth used in the line. i.e. if the size of the packet is more such as transferring or receiving huge files the utility of bandwidth is high, which impacts the latency. 

3.	Routing issues in the transmission path, instead of packet travelling from source to destination in a greater number of hops than expected, the latency will be higher.

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Check the latency time difference between the cloud network and edge network. The lower the latency time, the better the performance of network.

## Code.
We have used weather data set as our data set as we dont have enough time to deploy real sensors and get readings from that. we have also added delay in the program inorder to make it realtime. The delay added was only one second because we have many data rows and if delay is more it take so much time. 

## Outliers detection in IoT network and sensor data

A network has been proposed to send sensor readings over to the server, before sending the data to the server end, the data is checked for anomalies at the edge 
or in the cloud.

## Deployment

Add additional notes about how to deploy this on a live system


