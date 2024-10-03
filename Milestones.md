# Project Milestones

## Milestone #1: Template App Architecture Design
Before writing any code, the intended architecture needs to be designed & documented in the form of graphics, reports, specification documents, etc.
#### Subtasks:
- Create module relationship diagram.
- Create dataflow diagram.
- Create 4+1 architectural view model diagram.
- Create UI specification document with all widgets & theming capabilities called out.
- Create device firmware update (DFU) over-the-air (OTA) flow diagram(s).
- Create Bluetooth flow diagrams.
- Create communications protocol specification contractually agreed upon by mobile apps & embedded modules.
- Create PE Pub Sub Diagram

`Desired Milestone Completion Date: Early 08/2024`
<br>

## Milestone #2: Demo Mode UI App
Before adding Bluetooth functionality, we want to have a functioning demo app fully released. This allows us to showcase the UI, widgets, and intended functionality with mock/junk data before implementing any Bluetooth services.

#### Subtasks:
- Implement the various screens & widgets outlined in the UI specification document.
- Implement a 'Demo Mode' which samples the app, including sample data from the Pub Sub.
- Implement the theming structure for the app & widgets outlined in the UI specification document.

`Desired Milestone Completion Date: 10/01/2024`
<br>

## Milestone #3: Bluetooth & Connectivity
After releasing a demo app that we're happy with and finalizing the UI, it'll be time to add Bluetooth in.

#### Subtasks:
- Implement the BLE protocol as outlined by the communications protocol specificiation.
- Migrate communications library into the app architecture & implement the necessary functionality.
- Create necessary unit tests for the communications protocol.
- Implement the Device Firmware Update (DFU) and all necessary components.

`Desired Milestone Completion Date: 01/01/2025`
<br>

## Milestone #4: Comprehensive Test Framework
Testing will be added in all throughout development. However, the full extent of our test framework, with 100% code coverage, is not expected until the end of this project.

#### Subtasks:
- Create an extensive set of test suites to ensure consistent & accurate functionality.

`Desired Milestone Completion Date: 03/01/2025`
<br>

## Milestone #5: Finalized Documentation & Deliverables
This includes any final documentation for the project, as well as deliverables necessary for the University.

#### Subtasks:
- Polish/adapt any of the design diagrams into documentation.
- Document any missing components, test frameworks, etc.

`Desired Milestone Completion Date: 04/01/2025`