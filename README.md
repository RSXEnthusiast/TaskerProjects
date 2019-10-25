# CarBT

When my phone connects to BT it will turn off WiFi, crank the media volume, and give me 7 minutes to tap my NFC tag before disabling NFC.

When my phone disconnects from BT it will turn on WiFi and NFC, then kill my speedometer app and OBD2 monitoring app. I thought about killing google maps as well, but decided against it as sometimes I need to continue navigation after parking.

*Link to task download:*

https://taskernet.com/shares/?user=AS35m8nN4lm%2FP3ejzWzqBtCxdP081eI8WTJjbCeqK0tzhuKncN2vHnuw9Rq4T0dNsjcpbBVTouBI&id=Profile%3ARSX+BT+Connected

*Exported as Text:*

Profile: RSX BT Connected (6)

    	State: BT Connected [ Name:* Address:A0:14:3D:16:AF:0B ]
    
    Enter: RSX Connected (7)
     
     <Wifi Off>
    	
     A1: WiFi [ Set:Off ] 
    	
     A2: Wait [ MS:0 Seconds:7 Minutes:0 Hours:0 Days:0 ] 
    	
     <Max Volume>
    	
     A3: Media Volume [ Level:30 Display:Off Sound:Off ] 
    	
     A4: Wait [ MS:0 Seconds:0 Minutes:7 Hours:0 Days:0 ] 
    	
     A5: NFC [ Set:Off ] 
    
    Exit: RSX Disconnected (14)
    	
     <NFC On>
    	
     A1: NFC [ Set:On ] 
    	
     A2: WiFi [ Set:On ] 
    	
     A3: Kill App [ App:Car Scanner Use Root:Off ] 
    	
     A4: Kill App [ App:DigiHUD Pro Use Root:Off ] 
