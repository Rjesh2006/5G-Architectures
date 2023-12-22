# 5G Architecture Overview

## Service-Based Architecture

In the dynamic realm of 5G architecture, the interaction between network operations is symbolized through a service-based or reference point representation. Described in a service-centric manner, network functions (NF) play a pivotal role as service producers, offering capabilities to authorized NF service consumers through meticulously designed service-based interfaces.


***here you can seee hoe the exactly the architecture loking likr in this given figure:- by techcomunity.microsoft***

![image](https://github.com/Rjesh2006/5G-Architectures/assets/143868643/3893fb73-5681-432f-bb70-3b03f7dc6f9a)


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

# 5G Core Network

- Central hub for secure and reliable connectivity, offering access to all networking services.
- Software-based, native to the cloud for higher deployment agility.
- Crafted by industry experts following the 3GPP standard (5G core) to control and manage network functions.


