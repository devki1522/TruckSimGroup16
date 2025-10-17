# TruckSimGroup16
In this project we will use c# for coding. we will be applying our knowledge of TDD along with integration testing. we will also be developing a proper SRS and Flow chart diagrams for the project as well. 


Mini SDLC Due frifday October 17, 2025
Team Member assignments

1. Create a Github Repository            - ~~Devki~~
2. Finalize Team Charter                 - Devki (waiting on Nasir and Shreemn to sign the contract)
3. Create a project pitch                - ~~Devki~~
4. create a project plan                 - ~~Shumroz~~
5. write up the Requirments document     - ~~Devki~~
6. Product Description                   - ~~Devki~~
7. Product Diagram                       - Shumroz
  a. Flow Chart
  b. UML
  c. Class Diagram
  d. Sequence Diagram
8. Product Backlog                       - Shumroz
9. User Story Acceptence Criteria        - Shumroz
10. Risk Register                        - Nasir
11. Test Plans                           - Nasir
      a. Unit integration testing
      b. System testing
      c. Usability testing 


```mermaid
flowchart TD

A[Start System] --> B[Initialize SCADA & Connect Trucks]
B --> C[Receive Truck Status Data]
C --> D{Truck Idle?}

D -- Yes --> E[Assign Load via Dispatcher]
D -- No --> F[Monitor Active Trucks]

E --> G[Truck Executes Delivery]
F --> G

G --> H[Update Fuel, Location, Load Status]
H --> I[Store Data in Database & Update HMI]
I --> J{Any Alerts?}

J -- Yes --> K[Trigger Alarm & Notify Dispatcher]
J -- No --> L[Continue Monitoring]

K --> L
L --> M{Delivery Complete?}

M -- Yes --> N[Set Truck to Idle]
M -- No --> C

N --> C
C --> O[System Shutdown]
O --> P[Save Logs & Disconnect]
P --> Q[End]

```
