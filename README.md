# Capstone-Documentation

I had the pleasure to work on this project with 5 of my most talented colleagues from UBC ELEC, Bennett Galamaga, James Marx, Tenna Yuan, Callum O’Riley, and Suhail Khalil. While I am not at liberty to share everything, I would be happy to provide design files upon request. I have also included some of our key capstone design documentation, verification and validation is my favouriute because thats where you get to see how we confirmed all our claims. **Here are the highlights!**

We replaced a full silicon photonics lab spectroscopy setup with a single PCB, cutting the cost from $42,000 to just $700!

<img width="800" height="448" alt="image" src="https://github.com/user-attachments/assets/63095d9a-e4b0-486a-ac84-8945cc186157" />

We built a 4 layer PCB spanning 8 separate schematics with over 363 total components, conducting over 10 design reviews to ensure our client's specifications were met. 

This PCB integrated a thermally chirped laser, 16 photodiodes with low noise transimpedance amplifiers, and Peltier temperature controllers. We achieved 5X greater wavelength resolution than a benchtop tunable laser setup.

<img width="800" height="502" alt="image" src="https://github.com/user-attachments/assets/61900946-14c5-4eb0-bcc1-ac67cf02b40e" />

We tuned our temperature controllers by fitting a step response with MATLAB system ID, then converting the model to Z domain with bilinear transformations. The P I and D gains were determined by running a script to minimize integral square error with a maximum sensitivity constraint. Our laser temperature controller achieved under 1/1000C° stability during modulation, an order of magnitude better disturbance rejection than a lab grade controller. 

We implemented a custom firmware-software communication protocol, allowing for real time data visualization on a host PC, while simultaneously interacting with benchtop microfluidic instruments.

<img width="1140" height="865" alt="GREG screenshot" src="https://github.com/user-attachments/assets/4827fceb-3c7f-4316-8c3a-683edbcdb622" />

Our system is so convenient that some UBC researchers prefer using it over the $42,000 benchtop setup. Our work is currently pending publication.
