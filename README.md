[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/4L_6KTNY)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=17750297)
# Assignment: Build and Deploy a Keyword Spotting Model using Edge Impulse

## Overview
This assignment introduces you to the exciting world of **TinyML** and edge AI hardware by guiding you through the process of building a keyword-spotting system using **Edge Impulse**. You will deploy your model on both a smartphone and an Arduino Nano 33 BLE Sense board to evaluate its performance and usability on resource-constrained hardware.

---

## Objectives
1. Learn how to build and train a keyword-spotting model using Edge Impulse.
2. Deploy the trained model to both a smartphone and embedded hardware (Arduino Nano 33 BLE Sense).
3. Analyze and report on the model's performance, including trade-offs between accuracy and inference speed.

---

## Steps to Complete the Assignment

### **Part 1: Train and Deploy Your Model**

1. **Create an Edge Impulse Account**:
   - Go to [Edge Impulse](https://edgeimpulse.com/) and sign up.
   - Create a new project.

2. **Follow the Tutorial**:
   - Complete the Edge Impulse tutorial on building a keyword-spotting model:  
     [Responding to Your Voice](https://docs.edgeimpulse.com/docs/tutorials/end-to-end-tutorials/responding-to-your-voice).

3. **Deploy to Your Smartphone**:
   - Follow the tutorial to deploy the model to your smartphone:  
     [Using Your Mobile Phone](https://docs.edgeimpulse.com/docs/development-platforms/using-your-mobile-phone).

4. **Bring Your Laptop**:
   - Deployment is quick (less than an hour), but ensure you have your laptop with you.

---

### **Part 2: Deploy to Arduino Nano 33 BLE Sense**

1. **Required Hardware**:
   - Use the **Arduino Nano 33 BLE Sense** board, (only 2 boards available) as part of the TinyML Arduino Learning Kit, which includes:
     - 1 Arduino Nano 33 BLE Sense board
     - 1 OV7675 Camera
     - 1 Arduino Tiny Machine Learning Shield
     - 1 USB A to Micro USB Cable  
     *(Use only the Arduino Nano 33 BLE Sense board for this assignment.)*

2. **Install the Arduino IDE**:
   - Download and install the Arduino IDE: [Arduino IDE](https://www.arduino.cc/en/software).

3. **Set Up Arduino IDE**:
   - In Arduino IDE, navigate to **Tools > Boards > Boards Manager**, search for `nano 33`, and install **Arduino Mbed OS Nano Boards**.
   - Select the Nano 33 BLE Sense board from **Tools > Board**.

4. **Prepare and Deploy the Model**:
   - After training in Edge Impulse:
     - Navigate to the **Deployment** page.
     - Select **Arduino Library** and choose **INT8 Quantization**.
     - Click **Build** to download the deployment ZIP file.
   - In Arduino IDE:
     - Include the ZIP file as a library: **Sketch > Include Library > Add .zip Library**.
     - Exit and re-enter the Arduino IDE to ensure the library is loaded.
     - Open the example code from:  
       **File > Examples > YOUR_PROJECT_NAME_inferencing > nano_ble_33_sense > nano_ble_33_sense_microphone_continuous**.
     - Verify and upload the code to the board.
     - Open the serial monitor (**Tools > Serial Monitor**) to observe outputs.  
       *(First-time compilation may take ~20 minutes.)*

---

### **Part 3: Resources**
- **How to Deploy a Model to Arduino**:  
  [YouTube Video](https://www.youtube.com/watch?v=uUh61R8Hu0o)
- **TinyML on Arduino Using Edge Impulse**:  
  [Cytron Blog Post](https://www.cytron.io/tutorial/tinyml-on-arduino-using-edge-impulse) *(Optional: Try controlling an LED with voice commands.)*

---

## Deliverables
Submit a PDF file with the following:
1. **Questions**:
   - Does the model perform as accurately as expected on your smartphone? List a few methods to improve the model's accuracy.
   - When building a model for resource-limited hardware, how do you balance fast inference times with acceptable model accuracy? What trade-offs did you encounter?
   - Include screenshots of the training performance from **step 6** of the deployment process.
2. **Videos**:
   - Record and provide links to:
     - The keyword-spotting model working on your smartphone.
     - The keyword-spotting model working on the embedded Arduino board.
3. **Reflections**:
   - Share your experience deploying the model to your smartphone and Arduino board. Mention any technical difficulties or interesting observations.

---

2. **Compilation Time**:
   - Be patient during the Arduino IDE's first compilation; it can take up to 20 minutes.

---

Happy experimenting!















