# Reference point network architecture:--

## Fundamental Pillars in 5G System (5GS):

- **End-to-End (E2E) Network Slicing:**
  - Allows the creation of virtualized network slices tailored for specific use cases.
  
- **Service-Based Architecture (SBA):**
  - A modular approach for service delivery, enhancing flexibility and scalability.
  
- **Software-Defined Networking (SDN):**
  - Network management through software applications, improving network control.
  
- **Network Functions Virtualization (NFV):**
  - Virtualizing network functions to increase agility and resource utilization.

These pillars form the foundation to efficiently support the heterogeneous Key Performance Indicators (KPIs) associated with new use cases in the 5G landscape. The 5G Reference Network Architecture, specified by 3GPP, is a non-roaming architecture.

## Network Nodes:

- **UE (User Equipment):**
  - 5G smartphones or cellular devices connecting over the 5G RAN to the 5G Core.
  
- **gNB (Next-Generation Node Base Station):**
  - 5G base station utilizing New Radio technology.
  - Utilizes Software-Defined Radio (SDR) with various MIMO capabilities.
  - Supports both Stand-Alone (SA) and Non-Stand-Alone (NSA) deployments.
  
- **5GC (5G Core):**
  - Core network with advanced functionalities, supporting cloud-native architecture.
  - Functionalities include Authentication, Security, Session Management, Traffic Aggregation, etc.





![image](https://github.com/Rjesh2006/5G-Architectures/assets/143868643/209760df-63a5-4db8-8fc8-b6d3ccec1e43)


# Components of 5G Core


1. **UPF (User Plane Function):**
   - Responsible for packet forwarding and routing.
   - Performs packet inspection and Quality of Service (QoS) implementation.

2. **AMF (Access and Mobility Management Function):**
   - Manages access and mobility control.
   - Handles UE registration and terminates non-access stratum (NAS) signaling.

3. **SMF (Session Management Function):**
   - Manages and controls user plane traffic.
   - Handles session management within the network.

4. **NSSF (Network Slice Selection Function):**
   - Supports network slice selection.
   - Selects network slice instances to serve User Equipment (UE).

5. **NEF (Network Exposure Function):**
   - Exposes network capabilities and events securely.

6. **NRF (Network Repository Function):**
   - Maintains NF profiles and their functions.
   - Assists in discovering connections between network functions.

7. **AUSF (Authentication Server Function):**
   - Stores authentication keys to authenticate User Equipments (UEs).

8. **PCF (Policy Control Function):**
   - Maintains network policies to manage network behavior.

9. **UDM (Unified Data Management):**
   - Stores subscriber information.
   - Supports identification, access authorization, and billing.

10. **DN (Data Network):**
    - External network, often representing the Internet.

11. **AF (Application Function):**
    - Fulfills the role of an application server.
    - Interacts with the 5G Core to provide various services.

These components work collaboratively to ensure the effective functioning of the 5G Core network, supporting a wide range of services and functionalities.



  ***here you can see the reference pointarchitecture interface***
# 5G Interfaces

![image](https://github.com/Rjesh2006/5G-Architectures/assets/143868643/c855728b-afd6-41be-94b7-b0b537891247)


The 5G architecture includes several reference points (NG1 to NG15) that define interfaces between different network elements. Each reference point plays a crucial role in facilitating communication and coordination within the 5G network. Here is an overview of the key 5G interfaces:

1. **NG1:**
   - Reference point between the User Equipment (UE) and the Access and Mobility Management Function (AMF).

2. **NG2:**
   - Reference point between the gNB and the Access and Mobility Management Function (AMF).

3. **NG3:**
   - Reference point between the gNB and the User Plane Function (UPF).

4. **NG4:**
   - Reference point between the Session Management Function (SMF) and the User Plane Function (UPF).

5. **NG5:**
   - Reference point between the Policy Control Function (PCF) and an Application Function (AF).

6. **NG6:**
   - Reference point between the User Plane Function (UPF) and a Data Network (DN).

7. **NG7:**
   - Reference point between the Session Management Function (SMF) and the Policy Control Function (PCF).

8. **NG8:**
   - Reference point between the Unified Data Management (UDM) and the Access and Mobility Management Function (AMF).

9. **NG9:**
   - Reference point between two Core User Plane Functions (UPFs).

10. **NG10:**
    - Reference point between the Unified Data Management (UDM) and Session Management Function (SMF).

11. **NG11:**
    - Reference point between the Access and Mobility Management Function (AMF) and Session Management Function (SMF).

12. **NG12:**
    - Reference point between the Access and Mobility Management Function (AMF) and Authentication Server Function (AUSF).

13. **NG13:**
    - Reference point between the Unified Data Management (UDM) and Authentication Server Function (AUSF).

14. **NG14:**
    - Reference point between two Access and Mobility Management Functions.

15. **NG15:**
    - Reference point between the Policy Control Function (PCF) and the Access and Mobility Management Function (AMF) in a non-roaming scenario, or between V-PCF and AMF in a roaming scenario.
      

*The reference point representation of architecture follows traditional practices and provides a comprehensive view of the interactions between different elements in the 5G network.*


# Reference of data via:- #gigamon.com

**(https://docs.gigamon.com/doclib61/Content/GV-Cloud-OpenStack/5G-Service%20Based%20Interface%20Application.html)** 

