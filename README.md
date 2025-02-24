# 📞 Chat and VoIP Communication System  

This repository implements a simple **Chat and VoIP** communication system. It allows users to **send text messages, make voice calls, and test the microphone** through a custom-built Java application. The system utilizes **UDP-based messaging** for communication.  

## 📌 Overview  

The system consists of a **Java application** where users can:  
- 📨 **Send and receive text messages.**  
- 📞 **Make and answer voice calls.**  
- 🎙️ **Test microphone functionality for audio calls.**  
- 🔄 **Handle different call states**, such as **active calls, outgoing calls, incoming calls, and microphone testing.**  

The application is designed to work **over a network** using **UDP** for messaging and voice transmission. It includes components for:  
- 📤 **Sending and receiving messages.**  
- 📞 **Handling call setup and termination.**  
- 🎧 **Managing audio input/output.**  

---

## 💻 How to Run

### Prerequisites:
1. **Java Development Kit (JDK)**: The application is built using Java, so ensure you have the JDK installed on your system.
2. **Wireshark (Optional)**: Use Wireshark to inspect the UDP packets for better understanding of the communication process.

### Configuration
**You need to update the receiverAddress and ownAddress with correct IP addresses and ports. These are used for setting up the connections for both sending and receiving data.**
```java
// Change with correct address and ports
static String receiverAddressString = "ipAddress";  // Change with actual address
static String ownAddressString = "ipAddress";      // Change with actual address
static int receiverPort = 12346;                    // Change with correct port
static int ownPort = 12345;                         // Change with correct port
```

### Running the Application:
**Windows:**
```bash
cd C:\your-local-path\src\main\java && javac
com\cn2\communication\*.java && java com.cn2.communication.App
```

**Linux/MacOS:**
```bash
cd your-local-path/src/main/java && javac com/cn2/communication/*.java
&& java com.cn2.communication.App
```

---

## 🏗️ System Architecture  

The application consists of the following components:  
- 💬 **Chat Client**: Sends and receives text messages using **UDP.**  
- 🎙️ **Voice Client**: Handles the **sending and receiving of voice data** via **UDP.**  
- 🎧 **Microphone Testing**: Provides functionality to **test microphone input.**  
- 🔄 **State Management**: Manages various states, including **call initiation, active call, call termination, and microphone testing.**  

---

## 🔀 Running Multiple Instances  

To test the application with multiple users, you can:  
- 🖥️ Run the program on **different machines**.  
- 🏗️ Run multiple instances on **one machine** by specifying **different port numbers**.  

Ensure each instance has a **unique port number** for UDP communication.  

---

## ✨ Features  

✅ **Text Messaging:** Send and receive messages asynchronously using **UDP packets.**  
✅ **Voice Calls:** Capture audio from the **microphone** and transmit it in real-time.  
✅ **Microphone Testing:** Ensure **audio input functionality** before making a call.  
✅ **UDP Communication:** Efficient, **low-latency** messaging and voice transmission.  

---

## 📚 Acknowledgments  

- ☕ **Java**: [Java Documentation](https://docs.oracle.com/en/java/)  
- 🌐 **Wireshark**: [Wireshark for network analysis](https://www.wireshark.org/)  
- 🔧 **JDK**: [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html)

---
