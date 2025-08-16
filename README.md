Automated Pet Feeder System: Design and Implementation

This repository contains the design and implementation of a low-cost, programmable automated pet feeder system.

Project Overview

The primary objective of this project is to address the client's (a local animal shelter) need for a reliable and efficient automated feeding solution. This system aims to enhance operational efficiency and ensure consistent, reliable feeding practices within the shelter.

Key Features and Functionality

The automated pet feeder system is designed to provide the following core functions:

- Reliable Dry Kibble Dispensing: Dispenses dry kibble for both cats and dogs at user-customisable, scheduled intervals.
- Robust Monitoring Capabilities: Incorporates advanced monitoring to identify whether dispensed food has been consumed within specified time frames. This is crucial for tracking pet eating habits and general wellbeing.
- Immediate and Actionable Staff Alerts: Generates alerts to staff for various issues:
    - Food Not Dispensed: Alerts staff if a mechanical failure prevents food from being released.
    - Empty Food Tank: Notifies staff promptly when the food storage tank is depleted, preventing missed feedings.
    - Unconsumed Food: Triggers an alert if dispensed food remains uneaten, prompting staff to investigate the pet's well-being.
- Low-Cost Hardware Implementation Focus: The system design considers future implementation using affordable, off-the-shelf components to ensure economic viability for widespread shelter adoption.

Core Assumptions

The system's design and proposed solution are based on several key assumptions to simplify development and align with the low-cost requirement:

- Exclusive Dry Kibble Dispensing: The system is engineered solely for commercially available dry kibble, simplifying the dispensing mechanism and storage requirements.
- Consistent Electrical Power Supply: The system assumes continuous operation via a standard electrical wall outlet, eliminating the need for complex and costly battery or solar solutions.
- Low-Cost Sensor Utilisation: Monitoring relies exclusively on readily available, low-cost sensors, specifically a weight sensor for the food bowl and a simple infrared level sensor for the food storage tank.
- Timely Staff Response: It is assumed that animal shelter staff will respond promptly to system-generated alerts. The system identifies issues but does not possess direct animal health diagnostic capabilities; human intervention is indispensable for resolving critical feeding issues or addressing animal well-being concerns.

Inputs and Outputs

The system effectively interacts with its environment through various inputs and outputs:

Inputs

- Real-Time Clock: Provides exact feeding times based on user-defined schedules (HH:MM).
- User-Set Schedule: A list of pre-determined, customisable feeding intervals for the system to follow.
- Infrared Level Sensor: Checks the food storage tank to determine if it has sufficient kibble or if it's empty (True/False).
- Weight Sensor (Bowl): Measures the amount of food in the bowl to confirm dispensing and subsequently, if the kibble has been eaten (grams).

Outputs

- Dispensing Mechanism Activation: Physically dispenses dry kibble and activates an associated sound to alert the animal.
- Staff Alert (Displayed Messages & Sound Signals): Timely notifications to staff for critical issues:
    - Mechanical Failure: Alerts if the feeder is unable to dispense food.
    - Empty Food Tank: Notifies staff to refill the food storage tank.
    - Unconsumed Food: Prompts staff to investigate the pet's well-being if food remains uneaten.
- Timer Display: Shows how long food has been waiting in the bowl.

Assignment Context

This repository serves as a practical demonstration of the integrated problem-solving process, encompassing the following key steps as defined in the assignment:

1. Analysis and Problem Definition: Clearly outlining the problem statement, requirements, and initial assumptions.
2. Data Organisation and Description: Detailing all necessary inputs, outputs, and operational parameters.
3. Algorithm Design (Flowchart): Visualising the system's logic and flow using a comprehensive flowchart.
4. Solution Implementation (Word Coding): Translating the designed logic into a series of clear, modular tasks using plain English.
5. Testing and Refinement: Rigorously testing the solution with sample scenarios and suggesting improvements for enhanced reliability and efficiency.
