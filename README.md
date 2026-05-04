# 🚗 PLC Parking Counter System

## 📌 Overview  
This project implements a parking counter system using a Siemens PLC programmed in ladder logic. The system simulates a real-world parking lot using push buttons as inputs and LEDs as outputs to indicate parking availability and occupancy.

## ⚙️ Tools & Technologies  
PLC: Siemens S7-200 / S7-1200  
Software: STEP 7 MicroWIN  
Programming Language: Ladder Logic (LAD)  

## 🧠 Working Principle  
The system maintains a count of vehicles entering and exiting the parking area:

➡️ Entry Button Pressed → Counter increments (car enters). LED Q0.2 and  Q0.5 act like a barrier opening to let the car in/out.
⬅️ Exit Button Pressed → Counter decrements (car leaves) . LED Q0.0 and Q0.3 act like a barrier closed to avoid cars coming in/out

The system ensures:
- The count does not exceed the maximum parking capacity  
- The count does not go below zero  

### LEDs indicate the parking status:
- 🟢 Available (spaces remaining)  
- 🔴 Full (no spaces available)  

## 🔌 Hardware Abstraction  
Push buttons are used to simulate vehicle entry and exit, while LEDs represent the parking status (available/full). This allows testing of the logic without real sensors.

## 🔌 Inputs & Outputs  

Inputs  
Entry Push Button → Acts as a sensor sensing the vehicle is near the barrier . 
Exit Push Button → Acts as a sensor sensing that the vehicle has crossed the barrier. 

Outputs  
Green LED → Parking available  
Red LED → Parking full  

## 🔄 Features  
- Counter-based vehicle tracking  
- Overflow and underflow protection  
- Real-time parking status indication using LEDs  
- Simple and modular ladder logic design  
- Sensor-less simulation using push buttons
- The barrier doesn't open when no space avaliable inside.

## 🎥 Demonstration  

[▶ Watch Demo](https://github.com/user-attachments/assets/ad31d58b-ca95-4e7f-8846-e46f1e626b42)

## 📂 Repository Contents  
- PLC Program File  
- Project Documentation  
- Demo Video  

## 📁 Project File 
parking lot counter.mwp → Complete Siemens PLC project (open in STEP 7 / MicroWIN)  


## 🚀 Future Improvements  
- Sensor-based vehicle detection (IR/ultrasonic)  
- 7-segment or LCD display for slot count  
- Multi-level parking support  
- Automatic gate control system  
- Mobile or SCADA-based monitoring  
