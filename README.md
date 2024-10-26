**Best Practices for Enabling Bitlocker**

 1.  Ensure that the device has TPM 2.0 for maximum security.</br>
 2. Use Endpoint Security > Disk Encryption Profile to enable and configure Bitlocker.</br>
 3. Avoid assigning more than one Bitlocker profile to the same device. This will avoid policy conflicts.</br>
 4. Check the Encryption readiness status of the devices from Devices > Monitor > Device Encryption status to ensure the   device is compliant and meets the criteria before enabling Bitlocker.</br>
 5. Do not enable Bitlocker on a device with third-party encryption enabled on the drives.</br>
 If you have old devices without TPM, Do not enable Silent Bitlocker Encryption, as it is incompatible.</br>
 ![image](https://github.com/user-attachments/assets/d3ddda5c-0e18-4091-9039-f242a2d7c724)


Login to Intune admin portal at https://intune.microsoft.com</br>
Select **Endpoint security**</br>
Select **Disk Encryption** </br>
Click on **+Create policy** </br>
Select the Windows platform and select **Bitlocker** as the profile type.</br> and search for and Create</br>
![image](https://github.com/user-attachments/assets/c5e79842-c290-4cc2-9ff8-9833d612becc)

Give the policy a name and description</br>

![image](https://github.com/user-attachments/assets/7fc781b6-44be-4aea-9d5d-fb1d0a055814)

Next to **Configuration settings** > Drop down the **Bitlocker** > Configure the Bitlocker as shown below for silent encryption to process.
**Note: The red-highlighted sections are very crucial for silent encryption to suceed** 
![image](https://github.com/user-attachments/assets/b961611d-c593-4cad-ad93-abf29146646f)

Step 2: Configure the **Bitlocker Drive Encryption as below**
![image](https://github.com/user-attachments/assets/dac164db-ee7b-4d8d-b131-d3486783c2c5)
Step 3:Configure **Operating System Drives** as shown below.
![image](https://github.com/user-attachments/assets/76e41401-1497-47cc-8d89-1bd6d02869b3)
![image](https://github.com/user-attachments/assets/18c6005a-bf0c-4183-b876-8c7a9951d71f)

Step 4: Configure **Fixed Data Drives**
![image](https://github.com/user-attachments/assets/91fa3554-8c37-499a-a6cf-6bed5f4b95f6)

Step 5: The **Removable Data Drives** encryption not configured in this scenario
Next to **Assignments** tab to assign this policy to devices/device groups</br>
Proceed to the **Scope** and click Next and **Create**
.</br>
The devices in the assigned group would be encrypted the next time the devices check in with Intune portal and the bitlocker keys would show up under the devices **Recovery keys** in Intune portal</br>
You can also kick up a Sync from the device or Intune portal for faster processing. No user intervention is required at all. 

