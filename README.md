# Revit-Plugin
![image](https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/1ead64fa-e6a7-40d4-baaa-8efe305f6253)

## Check plugin's [Notion Wiki](https://www.notion.so/Plugin-code-explained-d024a574b4e743c08ceb2720be331387):

https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/3ceee052-6e0c-47fb-a9f0-53b99b2ae49b

# 🗺️ Short map for the documents 🗺️
📄[TabPanel](https://github.com/Strategie-Digitali/Revit-Plugin/blob/main/tabPanel.cs) 
---
![image](https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/69844ddd-628e-4c65-87d0-424304976ba9)
This one defines a Revit add-in that creates a custom ribbon tab with multiple panels and buttons, each executing different commands within the Revit environment.

📄[.addin](https://github.com/Strategie-Digitali/Revit-Plugin/blob/main/SDManifest.addin) </br>
---
.addin configures a Revit add-in named "SD tools", specifying its assembly location, unique ID, class name for loading, vendor information, and additional descriptions and links for help and vendor contact. It should be located under <b>C:\ProgramData\Autodesk\Revit\Addins\20xx\ </b> (The ProgramData folder is hidden by default).

📁[Commands](https://github.com/Strategie-Digitali/Revit-Plugin/tree/main/Commands)
---
These files define different parts of a Revit plugin that extends its functionality that are connected to buttons. They include commands for creating schedules from selected elements, changing elements' levels, and adjusting views and materials within a project. Each file encapsulates a specific task or feature, organized as classes implementing Revit's API interfaces to interact with the Revit environment and execute commands based on user input or predefined actions.</br> </br>
![schedule](https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/aafcd254-b7d1-43bc-864c-ae50f29adbf9)
![mouse](https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/06552e7c-e03c-4b32-af33-d6ea9b340a74)

📁[UI](https://github.com/Strategie-Digitali/Revit-Plugin/tree/main/UI)
---
These files represent the logic behind tools with user interfaces. In opposite to previous folder these files are integrating UI elements (defined in XAML) with back-end logic (defined in C#). The .cs (C#) files contain the logic for commands and interactions within Revit, such as manipulating document elements, handling user input, and executing specific tasks. The XAML files define the graphical user interface elements, like buttons, text fields, and layouts, which users interact with. Together, these files create a bridge between Revit's API and a user-friendly interface (a window). </br>
![excel](https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/94483005-821d-4170-afe1-7a1ee1cac1f8)
![manager](https://github.com/Strategie-Digitali/Revit-Plugin/assets/162335297/4372fa87-a551-4963-85be-93bd0c04caf6)



📄[UI Activator](https://github.com/Strategie-Digitali/Revit-Plugin/blob/main/UIActivator/UIActivator.cs)
---
This code activates user interfaces from the "[UI](https://github.com/Strategie-Digitali/Revit-Plugin/tree/main/UI)" folder and links them to the commands of the buttons on a Revit tab, allowing users to interact with various custom functionalities through beatiful dialog windows.

📁[Installers](https://github.com/Strategie-Digitali/Revit-Plugin/tree/main/Installer)
---
In this folder you can find the pre-created files for making an insteller for our plugin. [Inno Setup Complier](https://jrsoftware.org/isdl.php) that should be preinstalled to use these files and create <b>.exe</b> file. 
