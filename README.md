# Esprit_PostProcessor_RotaryClearance

## Scope
This repository is intended to display how to output program information at the beginning of a CNC program generated using Esprit. This post processor modification requires no input from the Esprit programmer. This post processor utilizes two passes through the post. The first pass extracts data that the user would like to be output at the beginning of the program and records within array variables. The second pass generates the G-code read by the machining center. During the second pass, the extracted information can be printed into the G-code file. In this example, if the work coordinate's rotary clearance value is set to a value of 0 or less, a the note will contain asterisks.

## Example

### Without Changes:
![Initial Code Image](/Example_Images/Initial.png)

### With Changes:
![Updated Code Image](/Example_Images/Updated.png)