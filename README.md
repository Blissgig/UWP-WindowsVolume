# UWP-WindowsVolume
This allows a UWP application to update the Windows Volume, as opposed to the Application's volume.

Thanks for the help of fellow Reddits for some of this information.

https://www.reddit.com/r/WPDev/comments/4e3086/windows_volume/

c# example:  

double volumeChange = 0.5;

//The return value is the new/updated Windows volume level
float fValue = VolumeControl.ChangeVolumeToLevel(volumeChange);
