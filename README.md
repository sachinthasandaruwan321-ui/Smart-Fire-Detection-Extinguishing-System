Description :

This Is Operated When The Camera Detect Fire(Using Image Processing) ,When Move The Helmet(it Has Mounted MPU6050)The Base Pan-tilt  Servo Moves It(right-Left & UP-Down).Then The Camera Meets The "Fire", First Beep The Buzzer & After 2 Seconds ,It(Servo And it Has Mounted Mini Pump's Tube) Stop And It Water Spray 6 Seconds The Identified Area Then Relies To The Normal Mode , It Can Easily Control Manually As Well(Has Joystick Controller To Right-Left & Up-Down Movements Of Pan-Tilt Servos,& 2 Push Buttons To Control To Water Spray

This Integrate When Detects "FIRE" Then Automatically Water Spray For 6 Seconds. Those are 2 Systems ,
Base System Components:
   Esp32 As Receiver(ESP32-S3): Connect With the Helmet Esp32 With MAC Address(ESPNOW) 
   2Buck Converters: To Volume Down 12V To 5V(Esp32 5in) & Other 12V To 6V(2 Servo Motors) 
   Pan-Tilt with Servos: To Up Down Movements 
   12V Mini Pump: When Camera Identify Fire And Buzzer On Then 6 Second Spray Water
   Buzzer: For Identify Fire When Camera Identify 
   MOSFET(IRLZ44N): To Control Mini Pump Pressure 
   Push Buttons: To Manually Control The On the Mini Pump (1 For High & Low Pressures)
   2 Joystick Controllers : To Manually Control Pan-Tilt Servo
 Helmet System Components:
   Esp32 As Transmitter: This Give To Base Esp32 TO Signal With (ESPNOW)
   Buck Converter: To Volume Down 12V To 5V(Esp32 5in)
   Gyroscope Sensor(MPU6050): To Give Signals To The Base Pan-Tilt To Move
   Camera Sensor(OV2640): To Identify Text "Fire" & Give A REd thread To Identify Fire 
 
Following Parameters :

First At All This System Develop To Only Fire Detect & Extinguish But , In This Case I really Used  Esp32 Cam To Identify The Fire(using Image Processing ), Unfortunately The System Has Detected The Yellow Colour Items As Fire , Then I Recognize "If I Use This, My Whole Project Can Fail " . Then I Used To Text Identify Command When See Letter As " FIRE " The System Detect This Letters As Fire.
  
