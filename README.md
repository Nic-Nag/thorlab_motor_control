# thorlab_motor_control

Uses the thorlab motor class written by Julian Fells (see below for link) to create a GUI that allows two rotation stages to be operated from matlab.

Depends on the thorlabs KINESIS drivers to operate, setup instruction for the motor class to opertate properly can be found at the link to the motor blass below.

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
 
