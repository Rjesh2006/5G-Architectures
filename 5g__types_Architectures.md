# 5G Architecture Overview

## Service-Based Architecture

In the dynamic realm of 5G architecture, the interaction between network operations is symbolized through a service-based or reference point representation. Described in a service-centric manner, network functions (NF) play a pivotal role as service producers, offering capabilities to authorized NF service consumers through meticulously designed service-based interfaces.


***here you can seee hoe the exactly the architecture loking likr in this given figure:- by techcomunity.microsoft***

![image](https://github.com/Rjesh2006/5G-Architectures/assets/143868643/3893fb73-5681-432f-bb70-3b03f7dc6f9a)

# Network Functions in 5G Service-Based Architecture

Assuming the role of either a service consumer or service producer, Network Functions are designed to be self-contained, independent, and reusable. Each Network Function service exposes its functionality through a Service-Based Interface (SBI), employing a well-defined REST interface using HTTP/2. To address issues related to TCP head-of-line (HOL) blocking, the Quick UDP Internet Connections (QUIC) protocol may be considered for future use.

## Components of 5G Service-Based Architecture

The 5G Service-Based Architecture (SBA) is composed of various components, including:

1. **Service Consumer/Producer Roles:**
   - Entities can take on the role of service consumers or service producers based on their requirements.

2. **Network Functions (NFs):**
   - Designed to be self-contained, independent, and reusable.

3. **Service-Based Interface (SBI):**
   - Each NF service exposes its functionality through a well-defined REST interface using HTTP/2.

4. **QUIC Protocol:**
  - Potential use of the Quick UDP Internet Connections (QUIC) protocol in the future to mitigate TCP head-of-line (HOL) blocking issues.

# 5G Network Elements and Their Functionalities in short terms:---

| Network Element                  | Functionality                                                     |
|-----------------------------------|-------------------------------------------------------------------|
| Access and Mobility Management Function (AMF) | - Access and mobility control.<br>- UE registration.<br>- Ends non-access stratum (NAS) signaling. |
| Session Management Function (SMF) | - Session management.<br>- Control user plane traffic.            |
| User Plane Function (UPF)         | - Responsible for packet forwarding and routing.<br>- Performs packet inspection.<br>- Implements Quality of Service (QoS). |
| Network Slice Selection Function (NSSF) | - Supports network slice selection.<br>- Selects network slice instances to serve User Equipment (UE). |
| Network Repository Function (NRF) | - Maintains NF profiles and their functions.<br>- Helps discover connections between NFs. |
| Network Exposure Function (NEF)   | - Exposes network capabilities and events securely.               |
| Unified Data Management (UDM)     | - Stores subscriber information.<br>- Supports identification, access authorization, and billing. |
| Authentication Server Function (AUSF) | - Stores authentication keys to authenticate UEs.               |
| Policy Control Function (PCF)     | - Maintains network policies to manage network behavior.          |
| Application Function (AF)         | - Fulfills the role of an application server.<br>- Interacts with 5GC to provide services. |
| gNodeB                            | - Hardware that connects to the network.<br>- Communicates wirelessly with UEs. |
| Data Network (DN)                 | - External network, such as the Internet.                         |




## Network Function Services

At the core of 5G's prowess lies the concept of Network Function Services. NF Service Producers act as virtuosos, endowing a spectrum of capabilities to their counterparts, the authorized NF Service Consumers. This orchestration takes place through service-based interfaces, unraveling multiple services, each adorned with a suite of procedures such as the nuanced choreography of NNRF MANAGEMENT and NBSF MANAGEMENT.

## Distinguishing 4G and 5G Network Architecture

| Feature                   | 4G Network                   | 5G Network                              |
|---------------------------|------------------------------|-----------------------------------------|
| Generation                | Fourth-generation network    | Fifth-generation network                |
| Max Download Speed        | 1 Gbps                       | 2.5 Gbps                                |
| Max Upload Speed          | 500 Mbps                     | 1.25 Gbps                               |
| Network Architecture      | Traditional RAN              | C-RAN (Cloud Radio Access Network)      |
| Modulation Techniques     | QAM and QPSK                 | Amplitude Phase-Shift Keying (APSK)     |

## A Deeper Dive

- **Cloud Radio Access Network (C-RAN):** The grandeur of 5G unfolds with the utilization of Cloud Radio Access Network (C-RAN), an architectural marvel where the centralization of baseband processing ascends to cloud-borne heights. This not only augments efficiency but also propels internet speeds into the realms of the extraordinary.

- **Modulation Poetry:** Where 4G found its expression in poetic modulation techniques like QAM and QPSK, 5G is set to compose a new verse with the avant-garde notes of Amplitude Phase-Shift Keying (APSK), promising a symphony of more efficient data transmission.

The transition from 4G to 5G is not just a leap but a symphonic crescendo, heralding higher speeds, reduced latency, and an unparalleled connectivity tapestry. 5G emerges as the maestro orchestrating the harmonies of the future, weaving together the threads of IoT, AR, VR, and beyond.


# 5G Network Functions Overview

## 1. NRF (Network Repository Function)
   - Centralizes storage for 5G NFs in the operator's network.
   - Provides a standards-based API for NF registration and discovery.
   - Crucial for the new service-based architecture (SBA) in the 5G core.

## 2. PCF (Policy Control Function)
   - Simplifies policy development and implementation in the 5G network.
   - Designed with cloud-native principles for 5G service demands.
   - Supports monetization and optimization of 5G capabilities.

## 3. BSF (Binding Support Function)
   - Comparable to 4G's Session Binding Function on the Diameter Routing Agent.
   - Becomes necessary with multiple PCF systems in the network.

## 4. SCP (Service Communication Proxy)
   - Grants routing control, resiliency, and observability to the core network.
   - Utilizes IT service mesh (ISTIO) for 5G-aware operations.
   - Addresses issues from the new SBA in the 5G core.

## 5. NSSF (Network Slicing Selection Function)
   - Chooses the best network slice for user-requested services in the 5G environment.

## 6. UDM (Unified Data Management) & UDR (User Data Repository)
   - Cloud-native, similar to LTE's Home Subscriber Server (HSS).
   - Manages credentials, authentication, and access based on user subscriptions.
   - Supports key 5G features, completing authentication and approving network access.

## 7. AUSF (Authentication Server Function)
   - Conducts 5G authentication and Key Agreement method (5G AKA).
   - Manages hidden or privacy-protected subscription identifiers during registration.
   - Selected by AMF (Access and Mobility Function) during registration.

## 8. NWDAF (Network Data Analytics Function)
   - Enhances end-user experience by streamlining key network data production and consumption.
   - Generates insights and addresses market fragmentation in network analytics.

# Benefits of 5G Service-Based Architecture (SBA)

The 5G Service-Based Architecture (SBA) represents a significant evolution in network capabilities tailored to the demands of the 5G era. The approach revolves around exposing Network Functions' (NFs) capabilities through Representational State Transfer (REST) APIs, utilizing the HTTP/2.0 protocol for enhanced efficiency and performance.

In the SBA framework, NFs' capabilities are presented through flexible interaction models, allowing for seamless integration between NFs based on either the Request/Response model or the Subscribe/Notify model. This flexibility accommodates the diverse needs of various 5G services, providing a versatile environment.

One of the notable advantages of SBA is its ability to cater to Application-driven Digital Service Providers. This support enables providers to achieve greater agility and faster time-to-market for the rollout of new products and services in the dynamic 5G landscape.

The modularity of NFs and their dynamic programmability are pivotal in the implementation of network slicing within the 5G architecture. This capability allows for the on-demand creation of multiple logical networks, serving different services simultaneously and contributing to a more efficient utilization of resources.

SBA further promotes openness by facilitating the unified incorporation of third-party applications with the core network. This inclusive approach supports multi-vendor plug and play solutions, enhancing the versatility of the network ecosystem.

To embrace modern deployment practices, SBA promotes a containerized and cloud-native approach for NFs. This deployment strategy not only fosters faster innovation but also expedites the overall service delivery process.

Feel free to utilize and customize this information for your Git repository README or documentation as needed.


# Reference of data via:--Calsoftinc.com #

(https://calsoftinc.com/blogs/2022/09/5g-service-based-architecture-sba.html) **Go through this website for more overview** 
