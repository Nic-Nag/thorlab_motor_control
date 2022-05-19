# thorlab_motor_control

Requirements:
- 'Driver for Thorlabs motorized stages', obtained through add-on menu in matlab
- DLLs from Kinesis, made available at https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=Motion_Control

In progress:

-Adding support for python wrapper to allow the app to target specific windows and send key presses which will allow some synchronisation of motor movements to various acquisition softwares. Currently being developed for NIS-Elements software so that Z-stacks can be acquired at different positions


Uses the thorlab motor class written by Julian Fells (see below for link) to create a GUI that allows two rotation stages to be operated from matlab.
The hardware support can be obtained by searching for 'Driver for Thorlabs motorized stages' in the add-ons section from matlab and downloading it.

Depends on the thorlabs KINESIS drivers to operate, setup instruction for the motor class to operate properly can be found at the link to the motor blass below.

Note that the MOTORPATHDEFAULT variable in the motor.m file from Julian Fells should be changed to teh director the location of the Kinesis DLLs on your machine. See link below for DLLs download location

===================
Acknowledged:
 Julian Fells (2022). Driver for Thorlabs motorized stages (https://www.mathworks.com/matlabcentral/fileexchange/66497-driver-for-thorlabs-motorized-stages), MATLAB Central File Exchange. Retrieved March 21, 2022. 
 
     % Download the Kinesis DLLs from the Thorlabs website from:
    % https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=Motion_Control
    % Edit MOTORPATHDEFAULT below to point to the location of the DLLs
    % Connect your PRM1Z8 and/or K10CR1 rotation stage(s) to the PC USB port(if
    % using PRMZ8 also switch it on)
===================    
    

 This GUI also provides an option to define a sequence of movements for the two motors.
 Serial numbers of the motors being used should be replaced with your own motor serial numbers in the script.
