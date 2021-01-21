## The Project - Fun with Quantum 

"Fun with Quantum" is a colletion of Jupyter notebooks that highlight specific aspects of Quantum Computing that are interesting and/or fun.


<img src="RasQberry.png" alt="hi" class="inline"/>


Quantum Computing - which is based on Quantum Mechanics - is a complex technology that is hard to understand for most people. Completely new algorithms - and even new thinking - is needed to exploit the potential power of upcoming quantum computers. This requires new approaches to teach Quantum Computing in engaging and understandable ways for IT experts, developers and young academics.

RasQberry integrates Qiskit, a Raspberry Pi (the full range from Pi 4 down to a Pi Zero) and a 3D printed model of IBM Q System One to explore various state of the art technologies and create a tool that can be used in meetings, meetups, demo booths, etc. A spectrum of Quantum Computing demos and Serious Games for Quantum Computing (that illustrate superposition, interference and entanglement) will be made available on this device for an engaging introduction to Quantum Computing. 



## Installation
### Qiskit on a Raspberry Pi


A first discription how to install Qiskit on a Raspberry Pi is available at (http://ibm.biz/Qiskit-Raspberry-Medium). It also includes a description how to setup some quantum demos (Qrasp, Raspberry-Tie) based on a Sense Hat 8x8 LED display. A summary of that article has been published at [hackster.io]: (https://www.hackster.io/news/jan-and-robert-lahmann-get-a-quantum-computer-running-on-your-raspberry-pi-in-under-30-minutes-4b972010009d)

 1. The medium article (http://ibm.biz/Qiskit-Raspberry-Medium) includes a "fastpass" at the end, and mentions a procedure that only requires very few commands 
    for the full setup.
    The following commands need to be executed in a terminal/ssh window on the Raspberry Pi with Raspberry OS "Buster".
    It will download and start a configuration tool "rasqberry-config", similar to the well known "raspi-config", that can be used to to some basic configuration,
    install Qiskit and several quantum demos.

     `pip3 install getgist
     `.local/bin/getgist -y JanLahmann RasQ-init.sh
     `. ./RasQ-init.sh

     Also use the `. ./RasQ-init.sh` command to start the rasqberry-config tool again or `sudo rasqberry-config`.
     
     <img src="rasqconfig-1.png" alt="hi" class="inline"/>

 2. "rasqberry-config" offers a simple menu structure. To setup RasQberry, go through the menu items in "S RasQberry Setup" one by one.
     Some of them require a reboot.

     Select either Qiskit version 0.19 or version 0.20 to be installed. "S6 Config & Demos" installs and configures some of the quantum demos.
     "D Quantum Demos" offers several Quantum demos, e.g. a Bloch Sphere demo (based on (https://github.com/JavaFXpert/grok-bloch) by James Weaver) 
     that runs on a TFT display attached to the Raspberry, and two demos that run on a SenseHAT display:

     [Raspberry-Tie] (https://github.com/KPRoche/quantum-raspberry-tie) by Kevin Roche and Qrasp (https://github.com/ordmoj/qrasp by Hassi Norlen).

     <img src="rasqconfig-2.png" alt="hi" class="inline"/>

 3. The above installation procedure used pre-compiled wheel files for most of the python packages. 
    These are downloaded automatically from  (https://www.piwheels.org). For the packages retworkx and qiskit-aer, currently there are no whl files available. 
    Total install with local compile takes 25 minutes on RPi 4, on a Pi Zero about 4.5 hours.
 

## The RasQberry 3D Modell

An enclosure (3D model) of the IBM Q System One can be used for RasQberry. STL files are available at (https://github.com/JanLahmann/RasQberry_enclosure) (original source: (https://github.com/BAndiT1983/RasQberry_enclosure). This is based on an idea of Andy Stanford-Clark (https://github.com/andysc/IBM-Q-System-One-3D-model). Additional instructions for assembling the enclosure and all components (Raspberry Pi, 4'' touchscreen display, battery pack inside the enclosure, etc) will be provided later. 

<iframe src="https://www.youtube.com/embed/QkLW0Yw_pmg" width="560" height="315" frameborder="0"></iframe>


<img src="RasQberry-3D-Model.png" alt="hi" class="inline" style="with: 50%; hight: 50%;"/>

You can use the [editor on GitHub](https://github.com/jim-cessna/Fun-with-Quantum/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/jim-cessna/Fun-with-Quantum/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
