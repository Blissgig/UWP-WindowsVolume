# UWP-WindowsVolume
This allows a UWP application to update the Windows Volume, as opposed to the Application's volume.

Thanks for the help of fellow Reddits for some of this information.

https://www.reddit.com/r/WPDev/comments/4e3086/windows_volume/

Special thanks to user Sunius for creating the base code
https://www.reddit.com/r/WPDev/comments/4kqzkb/launch_exe_with_parameter_in_uwp/d3jepi7

You will also need to set "unsafe" code option in the project.
In Visual Studio 2015 select the PROJECT menu, then at the bottom select <Project Name> PROPERTIES.  On the left is a series of menus, select BUILD.  Within the GENERAL section select the checkbox "Allow unsafe code"


c# example:  

//This value can be positive, to raise the volume, or negative to lower the volume.
double volumeChange = 0.5;

//The return value is the new/updated Windows volume level
float fValue = VolumeControl.ChangeVolumeToLevel(volumeChange);
