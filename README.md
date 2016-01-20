<h2> ITP Unconference 2016 </h2>  

<h3> Getting acquainted with the RaspberryPi </h3>  

---

<h4>A step-by-step guide to setting up your Pi</h4>
<p>This guide focuses on the Pi Models 1 & 2, not the Zero, and is an extensions of Surya Mattu's 2015 Unconference session ( which can be found here: https://github.com/samatt/RasberryPiSetup ).</p>
<p> As per Surya's repo, you can find a concise explanation of the difference between a Pi and Arduino:  </p>
https://blog.adafruit.com/2012/06/18/ask-an-educator-whats-the-difference-between-arduino-raspberry-pi-beagleboard-etc  

</p>Raspberry Pi's website explains the differences between the different models:  </p>
https://www.raspberrypi.org/documentation/hardware/raspberrypi/models/README.md  

---

<h5>What you'll need:</h5>
<ul>
  <li> A RaspberryPi</li>
  <li> A computer with an SD card reader </li>
  <li> An microSD card ( 8GB, class 6 ) is recommended.  *The class refers to the read/write speed of the card. </li>
  <li> USB cable </li>
  <li> A screen with an HDMI port</li>
  <li> An HDMI cable </li>
  <li> A USB keyboard </li>
  <li> A USB mouse </li>
  <li> An ethernet cable </li>
</ul>

---  

<h5>Step 1: Installing the OS</h5>
<p>Your Pi is small computer, and all computers need an operating system (OS) to be of any use, so let's install one. The first thing you need to do is format the SD card.</p>
<ul>
<li>Download the SD Association's Formatting Tool from https://www.sdcard.org/downloads/formatter_4/eula_mac/ </li>
<li>Install and run the Formatting Tool on your machine</li>
<li>Select "Overwrite Format"</li>
<li>Give the disk a name that'll be easy to identify ( I just called mine 'Pi' ).</li>
<li>Check that the SD card you inserted matches the one selected by the Tool</li>
<li>Click the "Format" button (Be patient, this can take a while if you have a large card).</li>
</ul>

<p>We're going to be installing the RASPBIAN JESSIE LITE (this is the command line only operating system).  Feel free to install any of the other OSs, but this guide will be covering the JESSIE LITE only.</p>
https://www.raspberrypi.org/downloads/raspbian/  

<p>Now we're going to be be writing the disk image, that you've just downloaded, onto the microSD card using the command line.</p>

*Extract the raspbian-jessie-lite.zip file.
*Drag the raspbian-jessie-lite.dmg file into/onto your desktop.
*Open up Terminal.  With the SD card still inserted in your laptop/computer, type the following command into your terminal window:
  <pre>diskutil list</pre>
*You should see something like this:
[!Terminal](images/terminal.jpg)
*The easiest way to identify which disk is your SD card is to look for the name you gave it during formatting. You should also recognise it based on its size ( mine's a 16GB card ).
