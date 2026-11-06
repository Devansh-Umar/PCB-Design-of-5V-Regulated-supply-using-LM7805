# My First PCB Design – 230V AC Mains to 5V DC using LM7805 

I wanted to learn PCB designing to understand how an idea can eventually be converted into a physical board.

Initially, I thought of starting with my last **[BC547 Logic Gates Project](https://github.com/Devansh-Umar/Digital-Logic-Gates-Using-Discrete-BC547-Transistors)**, which involved 23 transistors. But then I realised that making my first PCB with 23 transistors might turn into a whole disaster! 😂

So, I thought, why not start small?

That's why, I decided to extend my previous **[Regulated Power Supply Project](https://github.com/Devansh-Umar/5V-Regulated-Power-Supply-using-LM7805).** First, I simulated the circuit, then built it physically using a breadboard, and now I've taken it one step further by designing its PCB.

## About the Project

My idea was simple just replicating my existing 230V AC to 5V DC power supply circuit and convert it into a PCB.

Since it was primarily for learning, I kept the original circuit topology instead of making it unnecessarily complicated by ignoring real transformer size, heat-sink, or electrical isolations.

### Components Used

| Component | Description |
|:---:|:---:|
| T1 | Step-down transformer |
| D1–D4 | 1N4007 bridge rectifier |
| C1–C3 | Filter and bypass capacitors |
| U1 | LM7805 voltage regulator |
| J1 | AC input terminal |
| J2 | DC output terminal |

## How Does It Work?

1. **Transformation:** Steps down the AC input and provides isolation.
2. **Rectification:** Four 1N4007 diodes form a full-wave bridge rectifier.
3. **Filtering:** Capacitors smooth the rectified DC and reduce ripple.
4. **Regulation:** LM7805 provides a fixed 5V DC output.

## PCB Designing Journey

The schematic part was relatively easy because I was already comfortable with the circuit.

But the real challenge started with PCB layout!

I had to understand footprint assignment, component placement, pin numbering and how electrical connections translate into copper tracks.

Honestly, track routing was probably the most underrated part of this entire process. It took me almost two full days to get the layout into shape.

After three complete restarts using KiCad's Global Deletions option to clear the tracks and start again, I finally ran the Design Rules Check.

**NOT A SINGLE ERROR! HOOORAAAHHH! 😂**


## Repository Contents

- [Gerber Files](Gerber_Files)
- [Drill Files](Drill_Files)
- [Schematic Views](Schematics)
- [Bill of Materials](Bill_of_Materials)
- [Final Wired View](Final_Routed_Tracks.png)
- [Both side PCB View](Front_Back_Board_View)

## What I Learned

- Working with schematic symbols and physical footprints.
- Component placement and PCB layout.
- Ratsnest connections and manual copper track routing.
- Design Rule Check (DRC).
- 3D PCB visualization.
- Gerber and drill file generation.

The biggest takeaway was understanding that drawing a circuit and designing a PCB for that circuit are two quite different experiences.

## A Little Preview 

Two full days of designing, routing, restarting and troubleshooting, compressed into just **44 seconds!**

That's the whole journey. 😁

[Just Hit Me](PCBDesign(7805).mp4)

## If you find this project useful, a star ⭐ on my repository would be memorable for me.
