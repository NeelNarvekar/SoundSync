<img align="center" width="624" height="351" src="https://i.imgur.com/J16GZ1i.jpg">

## What is Sound[Sync]?

**Sound[Sync]** is a web application that allows you to play songs simultaneously on multiple devices without having to pair them with each other. 

It is written purely in **HTML**, **CSS**, and **JavaScript** and uses voice commands to play, pause, and skip between tracks. Users can start blasting music simultaneously on any device that supports JavaScript by bringing all the devices close to each other and then simply saying the word "play".

## Why did we build it in the first place?

As college students, we understand that Bluetooth speakers can be expensive and that people don't always have them on hand for every occasion. We also know how frustrating it is to not be able to use speakers from all the devices that you usually have with you around campus. (laptops, phones, etc.)

Sound[Sync] makes it easy to collectively break out into song and jam with your friends on lazy afternoons. It's intuitive web interface coupled with voice recognition makes it a breeze to use while ensuring minimal latency so that you can enjoy a 360 degree audio effect while achieving virtually unlimited amplification.

## Technologies and libraries that fuel this project

Even though we tinkered around with a lot of JavaScript APIs and libraries over this 36 hour period, we were able to get a prototype up and running using only Annyang.js (for voice commands), WaveSurfer.js (to play and visualize the audio), and Granim.js (to customize the background on the web interface) in addition to the HTML, CSS, and JavaScript files we wrote ourselves.

## Challenges we ran into

Synchronizing time on systems that have completely different clock speeds and architecture is harder than we anticipated. We were initially relying on timers and/or getting time from a central server to get the devices to synchronize with each other so that they would start playing the song simultaneously and with low latency. 

We tried everything ranging from NTP (Network Time Protocol), to uploading local system time to a server and calculating and adjusting for latency by taking their difference. However, the fact that we couldn't ping servers as frequently as necessary to achieve no latency to play music seemed almost impossible. 

We also had a hard time coming up with an interface that felt intuitive to use. In the end, we ended up using voice commands to solve both of those problems.

## Accomplishments that we're proud of

We're really proud of the fact that we were able to run this natively just on a browser without having the devices explicitly communicating with each other. Not only does this remove the theoretical limit on the total number of devices that work in conjunction with each other (as seen in WiFi/Bluetooth Protocols), it also takes almost no setting up and effort to get it running. 

We were also really excited to be able to synchronize audio from a web browser on Windows, MacOS, and Android simultaneously. It was really cool to see up to 9 devices playing the same song in different parts of the room at once while we were testing it.

## What we learned

Due to the technologies we explored before settling on our final solution, we were exposed to a far greater amount of information than seen in just the final project alone. We learned about the difficulties involving pairing time and the libraries used to tackle this problem (like socket.io). In addition to this, we are now familiar with several audio libraries in JavaScript. This of course is in addition to the APIs and languages used in the project.

## What's next for Sound[Sync]?

Further applications of Sound[Sync] would include a collaborative playlist that each user would be able to contribute to. In addition to this, we would look into other technologies to further reduce the latency involved with playing audio from numerous devices. We are also planning to integrate the YouTube API to synchronize music videos over multiple devices.
