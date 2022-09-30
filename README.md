# Administrative-Units

# What is the purpose of administrative units?
- IT admins will use administrative units to isolate managing access. 
- For example, IT admins will create several administrative units for each department. 
- An administrator(s) will be assigned to manage one of the several administrative units

# In the below diagram:
- Administrative A contains a subset of users and will be managed by <em> only </em> Admin A
- Administrative B contains a subset of users and will be managed by <em> only </em> Admin B
- Administrative C contains a subset of users and will be managed by <em> only </em> Admin C

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167911618-d2fbf3cf-8ca5-42d1-b12f-9100bc65fbce.png" height="75%" width="75%" alt="Admin Units"/>
  
<p/>

# How to create administrative units?
- Navigate to Azure AD > Select Administrative Units blade > Add administative units

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167923436-9e09d8a2-b491-4b44-a9ce-c6dfe2788670.png" height="65%" width="65%" alt="Admin Units"/>
  
<p/>


# Use Case: 
- One department with two users and one group with two users with only one admin 
- One user in the Default Directory managed by Admin B


<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167935647-252e7b76-6c69-4707-b987-becd3306aeb7.png" height="65%" width="65%" alt="Admin Units"/>
  
<p/>

- Note that there are built-in Azure AD roles for only the Administrative Unit when one is created

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167939101-1fef01be-fcab-47b4-a6a3-2111ecabc719.png" height="125%" width="125%" alt="Admin Units"/>
  
<p/>

- Admin A can manage User A and User B and only the Logistics-Grp. Admin A cannot manage the users within the group.
- Below, Admin A, the owner of the group can add members or remove members

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167939960-6df25aac-01ab-4cf0-8d93-0e20e8f5564c.png" height="125%" width="125%" alt="Admin Units"/>
  
<p/>

Remember that Admin A, the owner of the Logistics-Grp who has User Administrator privileged for the Administrative Unit cannot manage User C, only the group.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167940287-49feb744-1804-4e6e-b5e5-6fade5a6df24.png" height="125%" width="125%" alt="Admin Units"/>
  
<p/>

- Admin B, the User Administrator for the whole directory, can manage both the users in the Administrative Unit and the users outside of the Administrative Unit.
- Below, Admin B can manage user A in the administrative unit.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167945208-ac2187fd-451f-43be-a236-d9a51d6e6847.png" height="125%" width="125%" alt="Admin Units"/>
  
<p/>

- Below, Admin B can manage user C in the logistics-grp

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167945459-a1e6a775-2dff-42b2-b647-c6335bbf5b75.png" height="125%" width="125%" alt="Admin Units"/>
  
<p/>

- Below, Admin B can manage the Logistics-Grp and add users to the group

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167945727-2989e5c8-3e9d-463f-8ce2-4d5305a6095b.png" height="125%" width="125%" alt="Admin Units"/>
  
<p/>

- Below, Admin B can also manage User E, who is not in the administrative unit.
- Note that the Admin of the entire directory may need to sign-out and then sign back in to fully recieve the permissions.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/167946372-faf86045-fb91-43b1-b7ca-a8b7365cb6d6.png" height="95%" width="95%" alt="Admin Units"/>
  
<p/>

# Remember
- The Global Admin role can manage all users. This role can add members to the administrative units and manage permissons.
- User Admins only manage users

