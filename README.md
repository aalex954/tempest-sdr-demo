# tempest-sdr-demo
TempestSDR attack performed using a HackRF, TempestSDR, and an HDMI 1.2 cable. 

## Background

TempestSDR is a side-channel attack technique that exploits the unintentional electromagnetic emissions from electronic devices. Using a HackRF SDR, an attacker positions the device near a target to capture these stray RF signals. These signals often correlate with the data transmitted such as the image on a screen or keystrokes from a keyboard. 
The captured signals are then analyzed and processed with specialized software (TempestSDR) to reconstruct the sensitive information. 

> This method, while powerful for demonstrating vulnerabilities in device shielding and emission controls, is strictly for controlled research or authorized testing, as unauthorized use is both illegal and unethical.

## Tempest SDR Project Overview

The Tempest SDR project is an experimental demonstration of how unintentional electromagnetic emissions from electronic devices can be intercepted and analyzed using a software-defined radio (SDR), typically with a HackRF device. Below is an overview of the process:

### 1. Scanning and Signal Identification
- **Wideband Scan:**  
  Use an SDR application or a spectrum analyzer tool to perform a wideband scan of the RF spectrum.

![WideBand Scan](https://github.com/user-attachments/assets/b4736a0b-a283-48cb-a5f4-6aaa06676ee0)


- **Signal Identification:**  
  Visually inspect the spectrum display to identify any anomalous signals, such as distinct peaks or unusual patterns. In this case, the goal is to detect a signal carrying a music tune.

![Test Pattern](https://github.com/user-attachments/assets/0a8fa2b6-5e7d-4d99-8bf0-cde5d94d4b0c)


![Signal Identification](https://github.com/user-attachments/assets/64f4a2c6-a80c-483d-bb0f-a022e7c09c78)




### 2. Driver Setup and Hardware Integration
- **HackRF Connection:**  
  Connect your HackRF SDR to your system.

- **Driver Installation:**  
  Ensure that the necessary drivers are installed so that the HackRF can reliably communicate with your SDR application.

![HackRF Connected](https://github.com/user-attachments/assets/f6804027-702c-4833-906b-ebf50a012044)


### 3. Tuning and Signal Processing in TempestSDR
- **Launch TempestSDR Application:**  
  Open the TempestSDR application after verifying that the HackRF is properly connected and recognized.
- **Frequency Tuning:**  
  Manually enter or select the identified frequency so that the HackRF tunes into that specific channel.
- **Signal Processing:**  
  The application applies digital signal processing techniques—including filtering, demodulation, and error correction—to extract and reconstruct the music tune from the captured RF emissions.

![Signal Tuning](https://github.com/user-attachments/assets/f6f4561b-91df-45ef-a054-ab9348f20991)


[Signal Tuning Video](https://github.com/user-attachments/assets/7e3ff363-8e6f-4c2b-a1c9-cd61a17954c6)



### 4. Analysis and Demonstration
- **Recovered Video Signal:**  
  Once processed, the output is the contents of the notepad application (username and testing), demonstrating how data (in this case, a video signal) can be inadvertently broadcast via electromagnetic emissions.

![Recovered Image](https://github.com/user-attachments/assets/470bb4b3-2fc3-4c0b-a672-d687cfe7923d)


- **Security Implications:**  
  This project serves as a powerful reminder of the importance of electromagnetic shielding and other security measures in electronic devices.

> **Note:**  
> Projects like Tempest SDR are intended for controlled research environments. Unauthorized interception or analysis of electromagnetic emissions is both illegal and unethical. Always perform such experiments with explicit permission and in accordance with local regulations.
