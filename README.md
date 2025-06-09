# DISCLAIMER
This is my first-ever project and also my first GitHub repository, so I’ll try to keep things as **simple and transparent** as possible—so both the person writing this (me) and the one reading it know exactly where we’re headed.

# INTRODUCTION

This project focuses on the design and simulation of a CMOS Inverter, a fundamental building block in digital electronics. The aim was to understand its working principles and go through the complete VLSI design flow, starting from schematic to layout and verification.
To achieve this, I used Xschem for schematic design and symbol generation, followed by **NGSPICE** for circuit simulation and waveform analysis. The layout was implemented using **MAGIC VLSI**,**NETGEN** also integrated open-source **PDKs-SKY130**.

## XSCHEM

[XSCHEM](http://repo.hu/projects/xschem/xschem_man/xschem_man.html) is a schematic capture tool used for designing electronic circuits. It's lightweight, fast, and well-suited for analog and mixed-signal design. Xschem allows users to draw circuits, define components, and generate netlists compatible with simulation tools like Ngspice.


## NGSPICE

![image alt](https://upload.wikimedia.org/wikipedia/commons/a/ad/Ngspice_logo.jpg)
[NGSPICE](https://ngspice.sourceforge.io/devel.html) is an open-source circuit simulation engine based on SPICE (Simulation Program with Integrated Circuit Emphasis). It is used to simulate analog, digital, and mixed-signal circuits. Ngspice takes netlists (like those from Xschem) and provides time-domain (transient), frequency-domain (AC), and operating point analyses.


## SKY130(PDK)

![image alt](https://user-images.githubusercontent.com/49194847/138075630-d1bdacac-d37b-45d3-88b5-80f118af37cd.png)
Sky130 PDK (Process Design Kit) is an open-source 130nm semiconductor process design kit released by Google and SkyWater Technologies. It contains all the necessary data—such as SPICE models, DRC/LVS rules, and layout files—for designing and simulating ICs (integrated circuits) at the 130nm node. It's widely used in education and open-source hardware development.


# BEGINNING 

Alright, so it all started when I was hunting for some projects to do over the summer break. That’s when I stumbled upon a video by the YouTuber **whyRD**, talking about how to get started with VLSI basics and what tools you'll need. It was the first time I heard words like Verilog, Xschem, and PDKs—and I had absolutely no clue what any of that meant. Naturally, I decided to see what the fuss was all about.

Fast forward through hours of intense Googling, heroic levels of procrastination, and diving deep into random internet threads—I finally got a grip on what I’d been missing out on.

I'll list all the steps which i figured i had to do to complete the set up of the open source softwares on my laptop and how to do it:

1.FINAL GOAL: Install **Magic VLSI**, **Xschem**, **NGSpice**, and the **Sky130 PDK**.

2.All of these tools are Linux exclusive, but luckily, that wasn’t much of a problem as Windows 11 provides **WSL (Windows Subsystem for Linux)**, which lets you run Ubuntu right inside Windows.Next up: installing all the free tools. I took help of YouTuber **Nurahmet Dolan** for initial setup.

3.Step-by-step process:
  → Get an error
  → Debug it
  → Get a new error
  → Debug that too
  → Missing files?
  → Reinstall everything
  → Surprise! Even more errors
  → Debug them
After surviving that loop a few (dozen) times... all the software was finally up and running. 🎉

Below attached picture is the basic commands and steps that i did
![image alt](https://github.com/saksham19rawat/CMOS_INVERTER/blob/main/CMOS%20INVERTER/WhatsApp%20Image%202025-05-19%20at%2016.47.21_49256d68.jpg?raw=true)


# Designing An Example Circuit

## opening xschem
![image alt](https://github.com/saksham19rawat/CIRCUIT-DESIGN-SIMULATION-TOOLS/blob/main/CMOS%20INVERTER/Opening%20xschem.png?raw=true)


![image alt](https://github.com/saksham19rawat/CIRCUIT-DESIGN-SIMULATION-TOOLS/blob/main/CMOS%20INVERTER/Home%20screen.png?raw=true)

## Designing a sample CMOS inverter

![image alt](https://github.com/saksham19rawat/CIRCUIT-DESIGN-SIMULATION-TOOLS/blob/main/CMOS%20INVERTER/EXAMPLE%20CIRCUIT.png?raw=true)

### NETLIST

![image alt](https://github.com/saksham19rawat/CIRCUIT-DESIGN-SIMULATION-TOOLS/blob/main/CMOS%20INVERTER/netlist.png?raw=true)

### NG-SPICE

![image alt](https://github.com/saksham19rawat/CIRCUIT-DESIGN-SIMULATION-TOOLS/blob/main/CMOS%20INVERTER/Using%20ngspice.png?raw=true)

### GRAPH

![image alt](https://github.com/saksham19rawat/CIRCUIT-DESIGN-SIMULATION-TOOLS/blob/main/CMOS%20INVERTER/EXAMPLE%20GRAPH.png?raw=true)









