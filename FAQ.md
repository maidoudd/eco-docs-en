# FAQ

### 1. Which browsers does Mi Eco Cloud website support?

At present, the PC version of Mi Eco Cloud website is adapted for Chrome and Firefox, while the mobile phone version is adapted for Chrome. We will contiously imporve the website's browser adaption in the future.

### 2. What is the difference between the "KSYun-Beijing6" and "AWS-Beijing" regions?

#### KSYun-Beijing6

Considering factors such as manufacturer support, business development, and operation costs, it is recommended that Mi Ecosystem enterprises and cooperation partners deploy the domestic cloud services of Chinese Mailand in KSYun-Beijing6 region. This region has User Management and User Pofile (Big Data) capabilities exclusively, and there is a dedicated circuit between Xiaomi's Machine Room and KSYun. The MIoT platform is only deployed in the Xiaomi's Machine Room. If you need to transmit data from MIoT to FDS (in Xiaomi's Server Room or AWS) and have higher requirements for network transmission, it is recommended that you use the AppEngine of KSYun-Beijing6 region and the FDS in Xiaomi's server room.

#### AWS-Beijing

For the businesses that do not depend on MIoT Platform, and non-real-time services without special requirements of transmission from MIoT to FDS in AWS, if having high reliance on Database and Redis/Memcached services, then it is recommended to deploy the could services in AWS-Beijing region (such as AppEngine, FDS, etc.).

### 3. How to control an application's extranet access?

You can choose different domain name types to control an application having extranet access or not. On KSYun / AWS console, you can determine the extranet or intranet access of an application via domain name selection. If the extranet access is prohibited, choose a private domain name for the application, otherwise a public domain name for it. Both public and private domain names can be set through security groups.

### 4. What is the time zone for the AppEngine?

The time zone is always UTC, whether the applcation is deployed on AppEngine in domestic or overseas regions.

### 5. What alert services does Mi Eco Cloud provide for users?

Mi Eco Cloud provides two different alert services for users:

* Both applications deployed in regions based on AWS and resources created with AWS sub-accounts can directly create CloudWatch email alerts.
* For applications deployed in regions based on KSYun, please contact Mi Eco Cloud team to configure the SMS alerts.
