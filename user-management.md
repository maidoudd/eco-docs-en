# User Management

## Overview

User Management includes the management of users, groups, and roles.  

- A user needs to be added into a specific user group to be able to login Mi Eco Cloud and control relevant resources. 
- A group is the owner of resources on Mi Eco Cloud and the object to granted permissions. 
- A role is a collection of permissions, including permissions for AppEngine, AppEngine (K8s), and User Profile, etc. Binding a role to a specific user group can control the user group's access to the resources owned by the group.

## 1. User

### 1.1 How do I create a user?

Login Mi Eco Cloud (cloud.mi.com) console, choose KSYun-Beijing6 region, and click "User Management".

![ ](/UM-1.png)  

After you enter the User Management page, switch to User tab and click "Create New User" button to create a new user.

![ ](/UM-2.png)  

## 2. Role

### 2.1 How do I create a role?

After you switch to Role tab, click "Create New Role" button to create a new role.

![ ](/UM-3.png)  

### 2.2 How do I add permissions to a role?

Select a created role, and add a permission of a specific service's sepecific resource to the role.

![ ](/UM-4.png)  

## 3. Group

### 3.1 How do I create a group?

After you switch to Group tab, click "Create New Group" to create a new group.

![ ](/UM-5.png)  
 Once the group is created, the next page will be the group detail page.

### 3.2 Binding roles to the group

On the group detail page, you can find the Role module. By clicking "Edit" and then "Add Role" buttons, you can add the roles to the group so that corresponding permissions will be granted to this group after saved.

![ ](/UM-6.png)  

## Tips

Before a user depolying applicaitons in AppEngine or AppEngine (K8s), the role bound with SpaceDeveloper permission of corresponding Space should be added to the group where the user belong.   
Before a user using User Profile services, the role having BIGDATA ACCESS_ALLOW permission of BIGDATA to the group where the user belong.
