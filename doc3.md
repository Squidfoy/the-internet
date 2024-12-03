# How does the internet work digitally?
Digitally, the internet trasfers data using **packets** and **protocols**.  
### Packets
A **packet** is a small piece of a larger set of data. You can think of packets as puzzle pieces that make up a larger puzzle. When data gets ent over the internet, it is broken up into these packets for the transfer and then reassembled at the destination.  
  
If all the packets are sent separite from eachother, how does the recieving computer know how to piece them together? Each data set is sent with a *header*, which is sent before all of the packets. The header contains information about the packets contents and also helps the recieving machine know what to do with the packets. The header acts as the instructions so that the recieving computer can reassemble and use the packets as efficiently as possible.  
  
Why use packets instead of transfering the entire data set? Some pieces of data are quite large, and trasferring it all at once would take a lot of time and may block the internet connection for others. Using packets allows data transfer to go more efficiently, decreasing network congestion and increasing transfer speed. Additionally, if any of the packets fail to send, the recieving computer is only missing part of the data rather than the entire data (and the missing packet can be sent again).
### Protocols

Click [here](README.md) to go back to the main page.
