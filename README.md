# Problem-with-attiny-mouse


In this Issue have a solution for problem with mouse in Attiny 85

I had the same problem how this
digistump/DigistumpArduino#63

The library is wrong
It is necessary change some lines

the correct is in line 254 until 264, need change these lines
file DigiMouse.h
In my laptop the address is
C:\Users\USER\AppData\Local\Arduino15\packages\digistump\hardware\avr\1.6.7\libraries\DigisparkMouse\DigiMouse.h

void rightClick(){
	last_built_report[0] = MOUSEBTN_RIGHT_MASK;
}

void leftClick(){
	last_built_report[0] = MOUSEBTN_LEFT_MASK;  //It was wrong in here
}

void middleClick(){
	last_built_report[0] = MOUSEBTN_MIDDLE_MASK;    //It was wrong in here too
     }

My profile in LinkedIn https://www.linkedin.com/in/mariliahoshino/

Personal page https://mariliahoshino.wixsite.com/cvitae

Instagram https://www.instagram.com/mari.zeniti/

Facebook https://www.facebook.com/mari.zeniti

In this Issue have a solution for problem with mouse in Attiny 85
