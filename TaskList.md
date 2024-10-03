## Task List
*All tasks will be assigned to Jeremy Oosterbaan, as he is designing, developing, & implementing this project solo for Performance Electronics, Ltd. (PE).*

### Preliminary
There is some preliminary groundwork that needs to be done as a prerequisite for starting this project. 
- Create GitHub/Bitbucket code repositories for each of the necessary libraries.
  - Bluetooth Library
  - Communications Library
  - DFU Libary
  - Pub Sub Library
  - REST Libary
  - State Library
  - Utility Libary
  - Widgets Library
- Create GitHub/Bitbucket code repository for the base project & import all necessary libraries as git submodules.
  - Template App
- Research different ideas for implementing various aspects of the project to make decisions about libraries or languages used, architecture or data models used, etc.

### Design
The project is thoroughly designed and thought through before any code is written. Thus, lots of diagrams & documentation need to be created.
- Create module relationship diagram.
- Create dataflow diagram.
- Create 4+1 architectural view model diagram.
- Create UI specification document with all widgets & theming capabilities called out.
- Create device firmware update (DFU) over-the-air (OTA) flow diagram(s).
- Create Bluetooth flow diagrams.
- Create communications protocol specification contractually agreed upon by mobile apps & embedded modules.
- Create PE Pub Sub Diagram

### Development
Design is broken into a couple stages, due to the compartmentalized nature of the architecture.

#### UI
Building the UI & 'Demo Mode' so that a *sample* of the app can be shown to possible customers.
- Implement the various screens & widgets outlined in the UI specification document.
- Implement a 'Demo Mode' which samples the app, including sample data from the Pub Sub.
- Implement the theming structure for the app & widgets outlined in the UI specification document.

#### PE Pub Sub
The PE Pub Sub is a universal, generic, & modular way of publishing/subscribing to events throughout the app. This mechanism is used for triggering various events in the app, updating data displayed, changing the app state, and more.
- Implement the PE Pub Sub library externally.
- Create a test suite to ensure consistency & accuracy in the PE Pub Sub library.
- Migrate the PE Pub Sub library into the app architecture itself and implement the necessary functionality.

#### Bluetooth Low Energy (BLE)
PE uses a proprietary bluetooth standard—outlined in the communications protocol specification and with parser(s) living in the communications library—to handled all of our communications over bluetooth.
- Implement the BLE protocol as outlined by the communications protocol specificiation.
- Migrate communications library into the app architecture & implement the necessary functionality.
- Create necessary unit tests for the communications protocol.

#### Device Firmware Update (DFU)
PE uses a proprietary device firmware update process designed to work with our modules. This process is implemented over various medians (conroller area network (CAN), serial, etc.) and needs to be implemented over bluetooth in Android as well.
- Implement the DFU process & design the necessary state machines.
- Create necessary unit tests for the DFU process and perform automated testing.

### Testing
Testing must continue to evolve & adapt across the entire development lifecycle. Thus, there is only 1 generic task that encompasses testing.
- Create an extensive set of test suites to ensure consistent & accurate functionality.

### Documentation
Documentation will continue to evolove & adapt across the entire development lifecycle.
- Polish/adapt any of the design diagrams into documentation.
- Document any missing components, test frameworks, etc.