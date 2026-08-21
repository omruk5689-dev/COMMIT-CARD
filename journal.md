# COMMITCard. Project Journal

| **Project Name**       Commitcard  |

| ---------------------- | ----------- |

| **Designing Software** | EasyEDA Pro

| **Time Taken**         | 1.5 Hours   |

| **Designed By**        | OMER     |

---
<img width="2160" height="1257" alt="3D_PCB1_2026-08-21" src="https://github.com/user-attachments/assets/5140fffc-f77a-471b-9904-9212acffd5ad" />

## Project Overview

COMMITCard is a small project that uses NFC technology on a PCB to make sharing my GitHub profile a bit more engaging.

The idea was simple: build a card that has an NFC antenna and a few basic electronic parts that a phone can read.

This project was mainly an experiment with PCB design, NFC and creating something that feels personal.

---

## 1.  Schematic. ~25 Minutes

I began by drawing the schematic in Pro.

First I searched for the components I needed:

* NFC antenna

* Resistor

* Capacitor

* LED

* Other required connections

After locating the components I put them into the schematic. Wired them together.

The schematic was quite simple so this part did not take long.

I mainly concentrated on ensuring each component was wired correctly before I moved to the PCB layout.
<img width="2362" height="1672" alt="SCH_Schematic1_1-P1_2026-08-21" src="https://github.com/user-attachments/assets/1548067a-c7cc-48be-bed1-5a278f9da703" />

---

## 2.  PCB Layout. ~35–40 Minutes

After finishing the schematic I proceeded to the PCB design.

First I drew the outline of the PCB board to give the card a basic shape.

Then I began placing the components inside the board.

When all components were positioned correctly I began routing the traces between them.

This is where I encountered my real problem.
<img width="2160" height="1317" alt="PCB_PCB1_2026-08-21" src="https://github.com/user-attachments/assets/78113d48-3c45-4854-b3a9-ecc9b5986611" />

###  Routing Error

While routing the PCB I saw that some connections were not working properly due to the design rules.

The track and pad settings in my design rules were larger than what the actual components could handle.

Because of this I received routing errors. Could not properly connect some of the components.

It took me a time to discover the cause of the problem.

After checking the settings and understanding the issue I changed the design rules to match the PCB and component requirements.

After changing the settings I could finish the routing normally.

---

## 3.  Graphics & Final Design

After the PCB was finished I worked on making the card look more personal.

I looked for graphics and images that would fit the project then added and adjusted them on the PCB.

This part was about placing everything correctly and ensuring the graphics did not interfere with the PCB design.

---

## 4.  Exporting the Project

After finishing the PCB design and checking everything I exported the required project files from Pro.

That marked the end of the COMMITCard project.

---

##  What I Learned

Even though COMMITCard is a simple project it gave me useful experience with the entire PCB workflow:

- **Schematic → PCB Outline → Component Placement → Routing → Design Rules → Graphics → Export**

The biggest thing I learned was that even a simple PCB can have configuration issues that take time to understand.

The routing error with the design rules was an example of that.

Overall it was a fun project and I liked the idea of turning something as simple, as an NFC tag into a physical card that represents my work.

---

### ️ Total Time

**Approximately 1.5 hours**

###  Designed By

**O M E R**
