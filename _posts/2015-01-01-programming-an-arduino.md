---
title: Programming the Arduino
---


Normally, if we wanted to program an Arduino (or any other computer for that matter) we would have to write some code to tell it what to do. This code has to be written in a very specific way so that the Arduino understands *exactly* what you want it to do.
 
This is what the code to blink an LED on and off looks like :

{% highlight c linenos %}
void setup() 
{
  pinMode(13, OUTPUT);      // Set pin 13 up as an output. 
                            // Pin 13 has an LED built in.
}

void loop() 
{
  digitalWrite(13, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);              // wait for a second
  digitalWrite(13, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);              // wait for a second
}
{% endhighlight %}


This is a bit of a confusing place to start if you have never done any programming, but luckily for us some clever folks in Spain have made a tool called S4A (or Scratch for Arduino) that let's us control the Arduino using custom blocks that they have added to Scratch. 