## User Docs
*Due to the nature of this project—being more of a template or library to aid development, rather than a deliverable product—user documentation is rather difficult & limited. The bulk of the available user docs can be found below. Moreover, due to the codebase being owned by Performance Electronics, Ltd. (PE), I am somewhat limited in the depth at which I can share user documentation.*

#### Getting Started
To use the Templated Android App Architecture, one must first gain an understanding of the architecture's structure. While an in-depth understanding isn't necessary initially, it is important to recognize the central libraries & their roles. From the [Architecture Diagram(s)](Design_Diagrams/Design_D3.png), the *PE Template App* is the primary repository of this architecture. This repo includes the necessary peripheral libraries via Git Submodules. Forking this repository will give you a local copy of the *PE Template App*, including all necessary submodules.

##### Getting Started Steps
1. Fork the *PE Template App* repository
2. Recursively clone the forked repo, which should automatically create subdirectories with the various git submodules
3. You're all set! Project-specific code/functionality belongs in your forked (& cloned locally) repository.
   1. [Here is an image](/Resources/ProjectModulesFileStructure.png) of what the project directory—after forking & cloning—might look like.

#### Code Organization
As mentioned above, it's important to understand what role each submodule plays in the larger architecture. Below is a brief description of what code lives in each library:
  - **Bluetooth Library** - Bluetooth communications, functionality, & endpoints
  - **Communications Library** - Extensive test suite & routing mechanisms for the PE communication protocol
  - **DFU Libary** - Device Firmware Update (DFU) process
  - **Pub Sub Library** - The custom Pub/Sub mechanism, enabling intermodular communication
  - **REST Libary** - REST API integration & functionality
  - **State Library** - Centralized data store
  - **Utility Libary** - Various utility functions & constants
  - **Widgets Library** - Library of importable widgets, used to populate various implementations of the architecture

#### Widgets Library
One of largest components of this project is it's collection of modular, *drag-and-drop* widgets. Naturally, a comprehensive UI specification document, outlining each of these widgets & highlighting all of their configurable attributes was created in conjunction. Unfortunately, due to legal reasons, the full spec can't be added to this repository. Nonetheless, a [shortened demo](/Design_Diagrams/--CAPSTONE_DEMO--%20WO240309_MobileAppDesign_R3.pdf) of the UI spec has been made publicly available. Moreover, I'll discuss a few key aspects & include some brief images below:
- Many of these widgets have built-in *help buttons*. Tapping on one of these will display a snackbar with useful information on how to use the widget, what it represents, etc. These help strings are also fully customizable, as some projects may require custom help messages.
  - [Example Help Snackbar](/Resources/EditDeviceNameHelpSnackbar.png)
- To get an idea of the UI spec, one of the widgets can be seen below. The same format & detail level exists for a couple dozen custom PE widgets, all created as part of this project:
  - [Edit Device Name Widget - Requirements](/Resources/EditDeviceNameWidgetRequirements.png)
  - [Edit Device Name Widget - Illustrations](/Resources/EditDeviceNameWidgetIllustrations.png)

#### Testing
Each of the libaries contains a test suite—some far more extensive than others, merely due to time constraints—in order to verify functionality & minimize bugs. Again, for legal reasons, the codebase is not present here so I'm not able to display the full extent of these tests in detail. An image of the *PE Comm Processing Library* test suite can be seen below, to get an idea of the typical layout:
- [PE Comm Proc Library Tests](/Resources/PeCommProcLibraryTests.png)