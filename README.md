# ACL-AccessControlLite
ACL (Access Control Lite) is a mini access-control platform that simulates a professional security system in a simplified, user-friendly way. 
It features a React single-page UI backed by a C# (ASP.NET Core) REST API and a SQL Server database.

Core Features:
1. User Authentication & Role-Based Access Control
    - Secure user authentication
    -  JWT based authentication between React frontend and ASP.NET Core API
    -  Role based authorization to restrict access to configuration and monitoring features
2. Configuration Page
    - Create, modify, and delete:
        - Panels (access controllers) 
       	- Readers (card readers / doors) 
       	- Inputs (door contacts, request-to-exit, sensors) 
        - Outputs (locks, alarms, relays)
3. Monitor & Control Page
    - Live device monitoring:
        - View real-time status of panels, readers, inputs, and outputs 
        - Show online/offline, alarm, and normal states 
    - Manual control: 
        - By selecting the devices, a user will be able to simulate events/state of the devices. '
        - When a user clicks on a device, a control menu shoud be displayed where a user is able to do the follwing:
              - Set status online/offline
              - Open Door
              - Activate/Deactive
              - etc..
        - When a user selects a cardholder, they can simulate cardholder actions such as swipe badge at reader
        - Acknowledge / clear alarms or events
4. Backend & API
    - C# backend using ASP.NET Core to handle business logic and device simulation
    - RESTful API exposing endpoints for: 
        - Managing panels, readers, inputs, and outputs 
        - Querying device status and events 
        - Sending control commands
    - SQL Server database storing: 
        - Device configuration 
        - Event and state-change logs
5. Maybe a ChatBot feature??
