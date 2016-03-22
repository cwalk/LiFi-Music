## Introduction
Transmit music file over the visible light spectrum using LiFi (Visible Light Communication) to a speaker.

## Summary

There is actually no code associated with this experiment, it's done entirely through a circuit, and electrical engineering knowledge. I will attempt to explain the circuit below. It contains two parts, the phone circuit, and the speaker circuit.

## Phone Circuit

The Phone circuit contains these parts:

- Phone playing audio
- 3.5mm audio jack (with ground, left, and right wires stripped)
- 9V battery
- Breadboard and jumper cables
- LEDs
- Resistors
- Alligator Clips

I plug in the audio jack to the phone. I wire up the LEDs and resistors on the breadboard, with jumper cables to go to ground. Power -> resistor -> LED -> GND. Then, I attach the GND of the audio jack, to the GND of the breadboard. I then attach both the left and right of the audio jack to the GND of the 9V battery. I then attach the PWR of the 9V battery to the PWR on the breadboard. 

You should then see the LEDs all light up. This is simply applying power to the breadboard because the circuit is complete. If you unplug the audio jack from the phone, you will see the LEDs turn off. If you start playing a song, you will actually be sending the data through the LEDs, but you just dont have the speaker circuit hooked up yet, so you have no way to verify it's being sent, since the LEDs modulate too fast for the eye to see.

![Phone Circuit Diagram](/Phone Circuit.png?raw=true "Phone Circuit Diagram")

## Speaker Circuit

The Speaker Circuit contains these parts:

- Solar Cell (mine is 6V)
- Speaker (Mine is a powered bluetooth speaker, but I don't use the bluetooth at all. I simply use the audio in jack)
- 2 way 3.5mm audio jack
- Alligator Clips

Make sure your speaker has power, or is charged if it contains a battery. I use the "audio in" on my speaker, so I have a 2 way 3.5mm jack, which I plug 1 end into the speaker, and the other end I connect the GND (base) and PWR (tip) to the respective GND and PWR of the solar cell.

![Speaker Circuit Diagram](/Speaker Circuit.png?raw=true "Speaker Circuit Diagram")

## Usage

With these circuits complete, you should be able to hear the song through the circuit. If you dont, re-check the circuits, and use a multimeter to check to make sure you have sufficient current.

It helps if you point the LEDs directly at the solar cell. Also try with any surrounding lights off, to reduce noise from ambient lighting.

If you point the LEDs directly at the solar cell, you will hear the audio the loudest. You can also point the LEDs at an angle away from the solar cell, and hear it get quiter, but as long as the solar cell has sight of the LEDs light, it will still play the song. If you put your hand between the LEDs and the solar cell, covering them completely, you won't be able to hear the song, as the speaker can't recieve any of the data being transmitted from the LEDs.

I also used a simple tone frequency generator app on my phone, and sending 10Hz actually allows the human eye to see the LEDs modulating (they flicker). Anything 100+ Hz, the human eye won't be able to percieve.

## Science

What is happening (to my knowledge) is that we are taking a digital music file on the phone, and using the built in Digital-to-Analog converter to transfer the music to an audio jack. The audio jack is connected in series to a 9V battery, which is powering a breadboard with LEDs (with 220 Ohm resistors just so they don't short out).

As the analog output of the song changes, the LEDs modulate their output (they turn on and off really fast, faster than the human eye can see. It takes a really slow motion camera to pick it up, but it can be percieved slightly).

The second circuit is the speaker and solar cell. We use the solar cell as a reciever to pick up the song data being communicated by the LEDs (this could also be done with any photo-diode or photo-resistor). Then, that signal is processed by an amplified speaker, which allows you to hear the song being transferred through the LEDs. You can actually hear it through headphones instead of a speaker if you wish, but the sound is even more faint. I believe this to be because the speaker I use has power to it, so it acts like an "audio amplifier." 

- FYI I am not an electrical engineer by trade or education, so I'm not 100% on the science behind it, but this is my simple reasoning. I also used a nonpowered speaker, and could only hear static. It was too weak to hear the audio signal.

## YouTube

YouTube: 


## Pictures

Here are some extra pictures so you can see what my experiement looked like, if you are too lazy to watch the YouTube video above :P
