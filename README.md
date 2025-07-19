# Monitoring Temperature on 7-Segment
</br>

This project contain a code based on connection between TM1638 , Esp8266 , SHT20 and a 7-segment (LTD-322KD-31);
</br>
that monitoring Temperature and Humidity on serial monitor and shows the temperature on 7-segment.
</br>
</br>

# This is how it starts:
</br>

If the Temperature going ahead of 28°C , The LED lights up And its brightness is affected by temperature changes.</br>

If the temperature rises above 47°C, the LED will start flashing until the temperature drops below 47°C.</br>

When the device starts working, information about the ambient temperature and humidity is received by the SHT20 </br>

and sent to the ESP8266. Then, by connecting this component and the TM1638, the temperature Value is displayed on the 7-segment display.</br>
</br>


# List of Libraires which used in this code :
</br>

1- DFRobot_SHT20.h
</br>

2- TM1638.h

</br>
</br>

*** you can read other discriptions about some parts of the code in below link : </br>

<< https://github.com/Sobhanht/Brightness_Temp/blob/main/README.md >>
</br>
</br>
# Hints :
```C++
byte getBinaryForNumber(int num) {
   switch (num) {
    case 1: return 0b11000000;
    case 2: return 0b10110111;
    case 3: return 0b11010111;
    case 4: return 0b11001001;
    case 5: return 0b01011111;
    case 6: return 0b01111111;
    case 7: return 0b11000100;
    case 8: return 0b11111111;
    case 9: return 0b11011111;
    case 0: return 0b11111110;
    default: return 0b00000000;
  }
}
```







