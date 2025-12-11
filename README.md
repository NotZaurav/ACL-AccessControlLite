# ACL-AccessControlLite
ACL (Access Control Lite) is a mini access-control platform that simulates a professional security system in a simplified, user-friendly way. 
It features a React single-page UI backed by a C# (ASP.NET Core) REST API and a SQL Server database.

Core Features:
1. Configuration Page
    - Create, modify, and delete:
        - Panels (access controllers) 
       	- Readers (card readers / doors) 
       	- Inputs (door contacts, request-to-exit, sensors) 
        - Outputs (locks, alarms, relays)
2. Monitor & Control Page
    - Live device monitoring:
        - View real-time status of panels, readers, inputs, and outputs 
        - Show online/offline, alarm, and normal states 
    - Manual control: 
        - Trigger outputs (unlock door, activate relay
        - Acknowledge / clear alarms or events
3. Backend & API
    - C# backend using ASP.NET Core to handle business logic and device simulation
    - RESTful API exposing endpoints for: 
        - Managing panels, readers, inputs, and outputs 
        - Querying device status and events 
        - Sending control commands
    - SQL Server database storing: 
        - Device configuration 
        - Event and state-change logs

