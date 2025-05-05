# Security Assessment: Cedar Grove Family Health

This is a security assessment for a mock business. Cedar Grove Family Health is a family medicine clinic offering adult care, pediatric medicine, women's health and prenatal services, basic lab testing and vaccinations, and telehealth appointments. The clinic has 24 employees and around 3000 active patients.


**Security Framework:** We will be assessing against CIS Controls Version 8, Implementation Group 1.

**Assessment:** Find the assessment spreadsheet at https://github.com/mhmich/security-assessment/blob/main/Assessment%20Mapped%20to%20CIS%20Controls.pdf


### High-level system architecture:
**1.	Electronic Medical Record (EMR) System**
* Hosted in the cloud (e.g., AWS or Azure)
* Used for storing patient health records (ePHI)
* Accessed by staff via secure login
  
**2.	Patient Portal**
* Web-based
* Allows patients to:
  * View records
  * Schedule appointments 
  * Message providers
* Tied to the EMR system

**3.	Telehealth Platform**
* Integrated 3rd-party vendor (e.g., Doxy.me)
* Used for video visits and remote consultations

**4.	On-Premises Network**
* Clinic has a small server closet with:
  *	Firewall and router
  * Wi-Fi access point (staff and guest network separated)
* Workstations at each exam room and front desk
* Local file server for internal docs (not ePHI)

**5.	Billing Software**
* Web-based SaaS tool
* Connected to EMR for claims submission
* Managed by 3-person billing team

**6.	Email & Productivity**
* Microsoft 365 for email and document collaboration
* MFA enabled for all staff
* Email encryption for messages containing ePHI



<img src=https://github.com/user-attachments/assets/830457a6-7000-4b6b-8b10-a1471e921eaf width="600"/> 



