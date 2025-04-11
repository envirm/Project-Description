# 🔐 Envirm: Smart Security & IoT Ecosystem

The envirm organization hosts a collection of repositories that collaboratively form an integrated system aimed at enhancing device and network security through AI-driven analysis, IoT integration, and user-friendly interfaces.​

## 📦 Repository Overview

### 1. Network-Packet-Analyzer

**Language**: Python​

**Description**: Simulates a firewall and intrusion detection system (IDS) that processes incoming network packets, identifies potential threats, and logs incidents.​

**Functionality**:

- Analyzes packet metadata (e.g., IP addresses, ports, protocols).​

- Detects threats such as port scans, DDoS attacks, and malware.​

- Maintains a list of blocked IPs and logs all decisions.​

- Exposes RESTful endpoints for integration with front-end applications.​

### 2. AI-Service

**Language**: Python

**Description**: Implements AI models for threat detection and analysis, providing intelligence to the Network-Packet-Analyzer.​

**Functionality**:

- Processes network data to identify anomalies.​

- Classifies traffic patterns and potential threats.​

- Outputs threat assessments with confidence scores.​

### 3. Locken-Mobile

**Language**: Dart​

**Description**: A mobile application designed to manage access to smart locks, integrating AI for enhanced security.​

**Functionality**:

- Controls smart lock mechanisms.​
- Utilizes AI for user recognition and authentication.​
- Provides real-time access logs and notifications.​

### 4. locken-block

**Language**: Go​

**Description**: Backend service supporting the Locken-Mobile application, handling secure communications and device management.​

**Functionality**:

- Manages smart lock states and user permissions.​
- Ensures secure data transmission between devices and the mobile app.​

### 5. tracken-iot

**Language**: C++​

**Description**: Firmware for IoT devices that monitor and report on environmental and security-related metrics.​

**Functionality**:

- Collects data from sensors (e.g., motion, temperature).​
- Communicates with central servers for data analysis.​
- Triggers alerts based on predefined security thresholds.​

### 6. envi-front

**Language**: TypeScript​

**Description**: Front-end application providing a dashboard for administrators to monitor and control the security ecosystem.​

**Functionality**:

- Displays real-time data from various system components.​
- Allows management of blocked IPs and review of threat logs.​
- Facilitates configuration of system settings and thresholds.​

### 7. Hyperledge-Gateway

**Language**: TypeScript​

**Description**: Acts as a gateway for integrating blockchain technology into the security system, ensuring data integrity and transparency.​

**Functionality**:

- Records security events on a blockchain ledger.​
- Provides verifiable audit trails for security incidents.​
- Enhances trust in the system's data handling processes.​

### 8. Face-classification-using-CLIP

**Language**: Python

**Description**: Demonstrates facial classification using OpenAI's CLIP model, potentially for biometric authentication within the security system.​

**Functionality**:

- Processes facial images to identify individuals.​
- Integrates with access control mechanisms for user verification.​

## 🧩 System Architecture

The Envirm ecosystem is designed with modularity in mind, allowing each component to function independently while contributing to the overall security infrastructure.​

### Data Flow

- IoT devices (tracken-iot) collect environmental and security data.​
- Data is sent to the Network-Packet-Analyzer for initial processing.​
- The AI-Service analyzes data for potential threats.​
- Identified threats are logged and, if necessary, IPs are blocked.​
- Administrators interact with the system via the envi-front dashboard.​
- Access control is managed through Locken-Mobile and locken-block.​
- All critical events are recorded on the blockchain via Hyperledge-Gateway.
