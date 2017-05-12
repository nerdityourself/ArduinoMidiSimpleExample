# ArduinoMidiSimpleExample
 Simple example of how to send midi messages with Arduino

This is an example of how to send two midi notes with Arduino.
In these project we did not use the official midi library, but we send a single message directly calling the write functions on the serial.
We create the simple function 

void MIDI_TX(byte MESSAGE, byte PITCH, byte VELOCITY)
{

  status1 = MESSAGE + midichannel;
  
  Serial.write(status1);
  
  Serial.write(PITCH);
  
  Serial.write(VELOCITY);
  
  }
  
  to do this.
  
  We connected to the digital pin 7 and 4 two push buttons. 
  Each buttons send a different note. If you want to add more buttons, just increase the array size as appropriate. 
  
