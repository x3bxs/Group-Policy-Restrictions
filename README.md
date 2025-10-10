# 🧭 Group Policy Restrictions

This repository demonstrates how to **create local users** and apply **Group Policy restrictions** in a Windows Server (or Hyper-V) environment.  
The screenshots below show the complete process — from creating users to applying and verifying GPO restrictions.

---

## 👤 Creating Users

1. Open **MMC (Microsoft Management Console)**.  
2. Select **File → Add/Remove Snap-in**.  
3. Choose **Computer Management** and click **Add**.  
4. Under **System Tools → Local Users and Groups → Users**, right-click and select **New User**.  

<table>
  <tr>
    <td><img width="400" alt="Creating User - Step 1" src="https://github.com/user-attachments/assets/bfb7c023-be7b-40ca-a755-046ca8671634" /></td>
    <td><img width="400" alt="Creating User - Step 2" src="https://github.com/user-attachments/assets/443e9acb-cd6a-4682-8589-3e565380b893" /></td>
    <td><img width="400" alt="Creating User - Step 3" src="https://github.com/user-attachments/assets/b2db6564-abc6-436d-9a18-40eb1cad211d" /></td>
  </tr>
</table>

---

## 🔒 Adding the Local Group Policy Snap-In

1. Open **MMC** again and select **File → Add/Remove Snap-in**.  
2. Choose **Group Policy Object Editor** and click **Add**.  
3. Click **Browse**, select the specific user account you created earlier, and apply the snap-in.  
4. Configure the **Group Policy settings** to apply restrictions for that user.

<table>
  <tr>
    <td><img width="350" alt="GPO Restriction 1" src="https://github.com/user-attachments/assets/89464fd9-4747-4782-aa18-b671634c46e6" /></td>
    <td><img width="350" alt="GPO Restriction 2" src="https://github.com/user-attachments/assets/68210f94-614e-4fbd-93db-accd545291ac" /></td>
    <td><img width="350" alt="GPO Restriction 3" src="https://github.com/user-attachments/assets/2f5f4cdf-7048-4fd3-90b4-992e41ea8bbe" /></td>
  </tr>
  <tr>
    <td><img width="350" alt="GPO Restriction 4" src="https://github.com/user-attachments/assets/44296e2d-1097-4543-8fdc-a3a638c246ca" /></td>
    <td><img width="350" alt="GPO Restriction 5" src="https://github.com/user-attachments/assets/cf505ddb-afb4-42e8-ba7b-1c938ab3b03b" /></td>
    <td><img width="400" height="248" alt="GPO Restriction 6" src="https://github.com/user-attachments/assets/a7e9ae75-18b5-4eb5-a4d8-2fe9818e8c28" /></td>
  </tr>
</table>

---

## 🖥️ Applying Policies

Navigate to **Administrative Templates** within the **Group Policy Editor**.  
This section contains the full set of configurable policies that can be used to **restrict or customize user access**.
Screenshot below shows an example of **multiple policies** applies to the user.
<table>
  <tr>
    <td><img width="500" alt="Administrative Template - Example 1" src="https://github.com/user-attachments/assets/bf3d3832-d8a7-49be-9de1-d72fb94b9130" /></td>
    <td><img width="1209" alt="Administrative Template - Example 2" src="https://github.com/user-attachments/assets/4527d6b0-a557-48b7-85c0-a2ea1983a0c1" /></td>
  </tr>
</table>

After applying the desired restrictions, **log in to the target user account** (either locally or remotely) to verify that the configured policies have taken effect.

----

## 🖥️ Summary

- Created new user accounts within **Local Users and Groups**.  
- Added **Group Policy Object (GPO)** snap-ins to apply user-specific restrictions.  
- Configured and tested policies within **Administrative Templates**.  
- Verified enforcement either by loging into user or **Group Policy Management Console (GPMC)**.  


---

<div align="center"> 🖥️ Systems Management Projects 🖥️ </div>

