
# IEC 61499 control applications for FactoryIO scenes

A repository of IEC 61499 control applications developed using Function Blocks to control various industrial use case scenarios provided in the form of FactoryIO scenes. The control application uses OPC UA communication protocol to interact with the FactoryIO scene.




## Documentation

[FactoryIO Scenes](https://docs.factoryio.com/manual/scenes/)

[FactoryIO OPC UA Driver Setup](https://docs.factoryio.com/manual/drivers/opc/)

[Eclipse 4diac Download](https://eclipse.dev/4diac/download/)

[Eclipse 4diac OPC UA Tutorial](https://github.com/eclipse-4diac/4diac-documentation/blob/main/src/communication/opcUA.adoc)


## Installation

 - Download Eclipse 4diac IDE and 4diac FORTE
 - Download and install FactoryIO
 - Download the project 
 - Copy the project folder into 4diac workspace
 - Import the project from the system explorer tab of the 4diac IDE


    
## System Configuration

Go to *System Configuration* and configure the hostname and port number of your FORTE. In case, you are running a local FORTE, you can leave the default configuration.
## FORTE Configuration

The launch configuration uses a local FORTE which should be located in the following directory path:

```bash
4diac IDE/
└── runtime/
    └── 4diacFORTE/
        └── forte.exe
```

Therefore, you should copy the executable FOTRE into the following directory. Alternatively, you can configure the path of the local FORTE from the *Run Configuration* by going through the following steps:

 - Open *Run Configuration*
 - Left click on *Start_FORTE*
 - click *Browse* for the *FORTE location* option and select the local FORTE

## Deployment

The project contains a *Run configuration* folder. You can use the *Start Application* (can be found under the dropdown menu of the run button) launch configuration to deploy your application in debug mode. It will start a local FORTE and deploy the developed application. 

Alternatively, you can manually start FORTE and deploy application from the *Run Configuration*.
## FactoryIO Setup

 - Copy the relevant FactoryIO scene from the *Scenes* folder to your local FactoryIO    directory
 - Open the scene in FactoryIO
 - Go to Driver and check the OPC UA node mapping
 - In case the pre-defined node mapping doesn't work, you can use the driver tutorial from FactoryIo to configure it manually
