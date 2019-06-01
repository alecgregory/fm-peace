# Introduction
This is the style guide for fm-peace modules, part of the fm-peace approach to building FileMaker solutions. A FileMaker module can only be described as being in the fm-peace style if it adheres to the rules in this guide.

# 1 About modules
fm-peace modules are building blocks for fm-peace solutions.

## 1.1 Module files

### 1.1.2 File name
File names must only include lower case letters, and underscores or dashes. The string -peace must be the last string before the file extension.

### 1.1.3 Number of files in a module
A module must be contained in a single file

### 1.1.4 Security

#### 1.1.4.1 File Access Protection
File access protection must be turned off.

#### 1.1.4.2 Protecting modules (optional)

Optionally, modules can be protected. Protected modules must have a password on the [Full Access] account. The account name on the [Full Access] account can be changed from the default. An account using a privilege set that allows access to the module must be included. The module file must be set to log in with this account automatically.

### 1.1.5 Creating files
Files should be created using FileMaker's Create New... wizard. The Blank option should be used for creating the file
