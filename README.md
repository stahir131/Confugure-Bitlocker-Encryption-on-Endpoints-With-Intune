Login to Intune admin portal at https://intune.microsoft.com</br>
Select **Devices**</br>
Select **Configuration** </br>
Click on **+Create New policy** </br>
Select the required platform and select **Template** as the profile type.</br> and search for **Endpoint protection** and Create</br>
Give the policy a name and description</br>
Next to **Configuration settings** > Drop down the **Windows Encryption** > Configure the as needeed

![image](https://github.com/user-attachments/assets/f9f99f33-cfa8-4a80-b68b-9e36eceba82a)

Next to **Assignments** tab to assign this policy to devices/device groups</br>
Users should receive Encryption notification on their device to click through to finish up encryption.</br>
After users complete this, the bitlocker keys would show up under the devices Recovery keys in Intune portal</br>

The bitlocker can also be set up under **Endpoint security** in Intune admin portal</br>
Select **Disk encryption** and complete the setup.
