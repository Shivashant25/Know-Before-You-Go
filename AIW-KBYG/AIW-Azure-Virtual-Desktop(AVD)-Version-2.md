# Known Issues and workarounds 

1. **Copy-Paste Issue**

    **If Copy paste doesn’t work, please try following:** 

      - Please check if Clipboard permissions are on **Allow**, if not then change it to **Allow**. 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-1.png?raw=true) 

      - After allowing the clipboard content if you are not able to Copy the Content from lab Guide into the VM using copy button, then select the content which you want to copy from lab guide then right click > Copy to copy the content and then try to paste at desired location in Lab VM. 
      
      - Try to refresh the page or try any other Web Browser. 
      
      - Check on Network bandwidth in your local System/Laptop. 

     If the above points don’t work, then directly connect to the Lab VM using Remote Desktop Connection using the **Credentials** provided in **Environment Details** page.  

      - Copy the **LabVM/JumpVM DNS Name, Username** and **Password** from **Environment details** page 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-2.png?raw=true) 

      - Search for **Remote Desktop Connection** App from Start Menu items and then select the **Remote Desktop Connection** App. 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-3.png?raw=true) 

      - Paste the **VM** **DNS Name** in Computer field and then, click on **Connect**. 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-4.png?raw=true) 

      - Click on **More choices**. 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-5.png?raw=true) 

      - Now, click on the **Use a different account.** 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-6.png?raw=true) 

      - Now, enter the **VM Admin username** and **password** which you have copied from Environment details page and click on **Ok** button. Please add dot and back-slash “**.\”** before the Admin username. 

         ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-7.png?raw=true) 

      - Next, click on the **Yes** button to accept the certificate and add in trusted certificates. 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-8.png?raw=true) 

      - If **LabVM** opens on full screen, then you can **Restore Down** the window. 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-9.png?raw=true) 

      - Split the Window from lab environment page to open the Lab guide in Separate Window. 

          ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-10.png?raw=true) 

      - Now, copy the lab environment URL from the list and open that inside the VM itself and then use the Vm on full screen. 

          ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/copypasteissue-11.png?raw=true) 
 
 1. **Azure API issue**: 

     - Due to recent changes in Azure api's, azure API's are taking some additional time to fetch the details of the resources . The validation steps might fail initially for the lab, if you re-run the steps again after 30-45 minutes later then it will succeed if there will be no configuration related issue with lab steps you performed.

1. The attendees may face issues while trying to access the environment, 
    - they can check to see if the VM is in the running state, if not they can start it from the Virtual machine tab. 
    - It could also be due to a duplicate window open in another browser, we suggest closing all windows and trying again. Or using a private window and clearing the cookies.  

1. **Lab 1 Exercise 1 Step 3**: 

   A. Project Details     

   **Location** – make sure this is the same as the region of the resource group to avoid any errors. 
   
1. **Lab 2(A)**:

   - After completing Lab 2(A), The data in Azure Insights won't be loaded immeditately. It might take some time to load the data. Please perform the Lab 2(B) at the last and check the data.

1. **Lab 3 Exercise 1**:
  
   - Attendee should perform this exercise in their Own **PC/computer/workstation** not in the **JumpVM**. Peforming this exercise in **JumpVM** will cause connection issues when try to access the the published applications using WVD Desktop Client. 

3. **Lab 3 Exercise 1 Step 13**: 

   - The attendee might get an error while signing into office, as the account cannot be used to activate office in a shared computer scenario. We can ignore this and proceed with the lab.  

1. **Lab 6 Exercise 2 Step 9**: 

   - If attendee is not able to add the role assignment to file share then: 

     - Attendee should make sure that step 7 of task 1 of exercise 5 has been performed. 

        - “In the storage account, click on Configuration present under Settings blade. Then scroll down and find the option Active Directory Domain Services (Azure AD DS). Select Enabled for it.” 

        ![](https://github.com/CloudLabsAI-Azure/Know-Before-You-Go/blob/main/Labs/images/wvd-issue6.png?raw=true)

1. **Lab 6 Exercise 2 : Validation Failure** 

   - If the validation fails, attendees should make sure that Storage File Data SMB Share Contributor role is assigned to the file share userprofile which is created as a part of the lab. 