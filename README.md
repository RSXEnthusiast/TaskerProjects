# InCarNFC

When I tap the NFC tag in my car my phone will automatically open my speedometer app or my Navigation app, and my OBD2 monitoring app. It does all of this using AutoInput. It also turns off NFC, NFC is turned back on when my phone disconnects from my car's BT, done in a different profile.

*Link to task download:*

https://taskernet.com/shares/?user=AS35m8nN4lm%2FP3ejzWzqBtCxdP081eI8WTJjbCeqK0tzhuKncN2vHnuw9Rq4T0dNsjcpbBVTouBI&id=Profile%3AIn+Car

*Exported as Text:*

Profile: In Car (10)

     Event: NFC Tag [ ID:0452648ADA6480 Content:* ]
     
    Enter: Driving (11)
   
     A1: Menu [ Title:Navigation? Background Image: Layout:IconGridMenu Timeout (Seconds):30 Show Over Keyguard:On Items:(3) ] 
     
     A2: Stop [ With Error:Off Task: ] If [ %Navigate eq -1 ]
     
     A3: Launch App [ App:DigiHUD Pro Data: Exclude From Recent Apps:Off Always Start New Copy:Off ] If [ %Navigate eq 0 ]
     
     A4: Launch App [ App:Maps Data: Exclude From Recent Apps:Off Always Start New Copy:Off ] If [ %Navigate eq 1 ]
     
     A5: Wait [ MS:500 Seconds:0 Minutes:0 Hours:0 Days:0 ] 
     
     A6: Launch App [ App:Car Scanner Data: Exclude From Recent Apps:Off Always Start New Copy:Off ] 
     
     A7: Wait [ MS:500 Seconds:0 Minutes:0 Hours:0 Days:0 ] 
     
     A8: AutoInput Gestures [ Configuration:Gesture Type: Swipe
    Start Point: 540,2279
    End Point: 540,1860
    Duration: 500 Timeout (Seconds):60 ] 
     
     A9: Wait [ MS:500 Seconds:0 Minutes:0 Hours:0 Days:0 ] 
     
     A10: AutoInput Action [ Configuration:Type: Id
    Value: net.oneplus.launcher:id/show_more
    Action : Click Timeout (Seconds):23 ] 
     
     A11: Wait [ MS:500 Seconds:0 Minutes:0 Hours:0 Days:0 ] 
     
     A12: AutoInput Action [ Configuration:Type: Text
    Value: Split Screen
    Action : Click Timeout (Seconds):23 ] 
     
     A13: Wait [ MS:0 Seconds:1 Minutes:0 Hours:0 Days:0 ] 
     
     A14: AutoInput Action [ Configuration:Type: Point
    Value: 540,1720
    Action : Click Timeout (Seconds):23 ] 
     
     A15: Wait [ MS:0 Seconds:1 Minutes:0 Hours:0 Days:0 ] 
     
     A16: AutoInput Gestures [ Configuration:Gesture Type: Swipe
    Start Point: 545,1180
    End Point: 545,722
    Duration: 500 Timeout (Seconds):60 ] 
     
     A17: NFC [ Set:Off ] 
