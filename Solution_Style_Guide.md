# Introduction
This is the style guide for fm-peace solutions. A FileMaker solution can only be described as being in the fm-peace style if it adheres to the rules in this guide.

# 1 About solutions
FileMaker solutions come in many forms. They can be located within the FileMaker platform (or a part of the platform), incorporate external data and services directly (through the External Data Sources feature) or indirectly (through APIs and other integrations). This diversity should not be an excuse for poor solution architecture. Rather, we should use good architecture to support diverse, unusual or technically ambitious solutions.

## 1.1 Solution files

### 1.1.2 File name
File names must only include upper and lower case letters, and underscores or dashes. The first letter of each word should be capitalized.

### 1.1.3 Number of files in a solution
There is no limit to the number of files in a solution aside from the technical limits of the platform. The number of files in a solution should encourage code re-use and aid solution maintainability.

### 1.1.4 File types
Each file in a solution must be one of the following types

#### 1.1.4.1 Persistent data files
Persistent data files are for storing solution data. They should not include any layouts aside from the FileMaker required default layout. They must not include end user layouts. They must not include any scripts unless required for native security account creation.

#### 1.1.4.2 Controller files
Controller files mediate access to persistent data files and/or external components. They should include solution (business) logic. They must not include end user layouts.

#### 1.1.4.3 User Interface (UI) files
UI files mediate user interaction with persistent data files, controller files and external components. They should not include solution (business) logic beyond what is required for user interaction to work.

#### 1.1.4.4 Launcher files
Launcher files assist entry into UI files. Any data used by a launcher file to assist entry into a UI file must be stored in a table. It must not be stored in a custom function, script or layout object.

#### 1.1.4.5 Self-contained files
Self-contained files include all the functions of persistent data, Controller and UI files in a single file. Self-contained files must not include FileMaker external data sources.

### 1.1.5 Creating files
Files should be created using FileMaker's Create New... wizard. The Blank option should be used for creating the file
