# ARDY
Contains examples for beginners
LED Library for Arduino - ezLED
This library is designed for Arduino, ESP32, ESP8266... to control LED: on, off, toggle, fade in/out, blink, blink the number of times, blink in a period of time. It is designed for not only beginners but also experienced users.

ezLED stands for easy LED, which mean that the library is easy to use.

Features
Turn on/off
Toggle between on and off
Fade in/out
Blink
Blink with the number of times
Blink in a period of time
Cancel the blinking or fading anytime
Support both control modes: CTRL_ANODE and CTRL_CATHODE
Get the on/off LED's states: LED_OFF, LED_ON
Get the operation LED's state: LED_IDLE, LED_DELAY, LED_FADING, LED_BLINKING
All functions are non-blocking (without using delay() function)
Easy to use with multiple LEDs
Available Functions
ezLED(int pin)
ezLED(int pin, int mode)
void turnON()
void turnON(unsigned long delayTime)
void turnOFF()
void turnOFF(unsigned long delayTime)
void toggle()
void toggle(unsigned long delayTime)
void fade(int fadeFrom, int fadeTo, unsigned long fadeTime)
void fade(int fadeFrom, int fadeTo, unsigned long fadeTime, unsigned long delayTime)
void blink(unsigned long onTime, unsigned long offTime)
void blink(unsigned long onTime, unsigned long offTime, unsigned long delayTime)
void blinkInPeriod(unsigned long onTime, unsigned long offTime, unsigned long blinkTime)
void blinkInPeriod(unsigned long onTime, unsigned long offTime, unsigned long blinkTime, unsigned long delayTime)
void blinkNumberOfTimes(unsigned long onTime, unsigned long offTime, unsigned int numberOfTimes)
void blinkNumberOfTimes(unsigned long onTime, unsigned long offTime, unsigned int numberOfTimes, unsigned long delayTime)
void cancel(void)
int getOnOff(void)
int getState(void)
void loop(void)
