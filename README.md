# Calculated Tampering 

A part of my project that I tried to keep closely coupled with the research/theory element was the application of these concepts. Ultimately I aimed to understand why specific design decisions were made by looking at a circuit board, maybe by also  probing some components. This would allow me to troubleshoot, improve, and hack devices in a calculated where an output would be expected. 

<img src="https://github.com/user-attachments/assets/6b1d2480-e061-42fb-964c-9b9eeba95baa" width="200">

To start I began with a Sony DAV-DX315 which is a home theatre system which I had thrifted. I did a complete teardown and upon inspection I was immediately caught by the 5 disc changer system. Typically they revolve the discs on a platter but this one would stack them in a magazine and retrieve or store a requested disc. I wanted to be able to control the disc changer stand alone so I tore it down as well. 

<img src="https://github.com/user-attachments/assets/c968e2e9-105c-4e0e-a54e-4b261cb7d421" width="200">

I found every switch and got an understanding of the disc changer where I was able to manually control the device. From here I needed to locate every switch and the purpose of every switch.
What was interesting about the system was the rotary switches it used to determine the position of the loading mechanisms and the magazine. After the full breakdown, it was time to reverse engineer the circuit by pulling up IC datasheets and creating a digital copy of the main circuit on Kicad to do so. 

<img src="https://github.com/user-attachments/assets/af637e3f-7488-4d09-baf4-064d6b895a8d" width="200">

Because of this and some additional checks around the board I was able to create a pinout and breakout board which would allow me to use an arduino to interface with the disc changer. Based on testing I had done on the rotary switch values I was also able to create a key to determine the position of the different parts of the disc changer. 

<img src="https://github.com/user-attachments/assets/9623bc7e-8ae3-4325-82d7-0c0ba2e2b018" width="200">
<img src="https://github.com/user-attachments/assets/7ab49f96-c543-48bc-9a0a-41b2ea908ee2" width="200">

With this I was able to control each individual action of the disc changer through an arduino, a benchtop power supply, and the new knowledge I had on the device. This was a valuable exercise in documenting a proprietary device on my own through knowledge I had gained in the research section 


## Laser Communicator

To conclude my junior project I wanted to create a small circuit without a microcontroller. Because time was running out I needed to create a device which was relatively simple yet demonstrated my understanding from the research part of my junior project. I created a laser communicator because I knew I could turn a yardlight, laser pointer, and some basic components I had on hand to create one.  

<img src="https://github.com/user-attachments/assets/30c0eee4-dd13-4203-bf86-bc5ae784e9e3" width="200">

At first the circuit was working, until it wasn't added I had to determine the issue. Building off of what I had previously learned and some additional research I decided to test the linearity between the laser and the solar cell which resulted in me unknowingly exceeding the laser diodes voltage rating and damaging it. This required me to redesign the common circuit with a photoresistor instead to get around this problem. 

<img src="https://github.com/user-attachments/assets/6e811c13-c00b-4134-9812-95ea0923ba71" width="200">
