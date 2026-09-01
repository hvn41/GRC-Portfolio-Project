# **Access Control & Authentication Policy** 

## **For User Credentials** 

### **Objective** 

To protect corporate user credentials and system access against unauthorized access, credential theft, and phishing risks. 

#### **Scope** 

Applies to: 

- All employees 

- Contractors 

- Third-party users accessing company resources 

#### **Requirements** 

##### **Multi-Factor Authentication** 

- Require mandatory Authenticator App for all external logins. 

##### **Password Requirements** 

- Minimum length of password is 14 characters 

- Password must include mix of upper- and lower-case letters, numbers, and special characters 

- Known compromised passwords are prohibited 

##### **Geographic Anomaly Detection** 

- Mandatory security alerts for logins originating from unexpected countries or new devices. 

##### **Incident Trigger** 

If credential compromise is suspected: 

- All active applications or VPN sessions must be terminated by IT department within 30 minutes of a reported or detected compromised. 

- Immediate inspection and removal of unauthorized malicious email autoforwarding rules or API keys created during the breach. 

- Immediate password reset must be forced across all applications (e.g. Google Workspace, Single Sign-On) 

- Multi-Factor Authentication must be permanently enabled and verified before account access is restored to the user. 

- Google Workspace admin must review logs for lateral movement, data access, or privilege escalation, covering a minimum of 30-day lookback. 

#### **Evidence Requirements** 

- Admin audit logs show the exact timestamp when active user sessions were revoked. 

- Automated system logs verifying that a forced password reset was initiated and completed. 

- Exported configuration logs confirming the audit and removal of any unauthorized email auto-forwarding rules. 

- User directory records prove active Multi-Factor Authentication status prior to account reinstatement. 

- A documented Incident Log detailing the log review, lateral movement checks, and root cause analysis. 

#### **References** 

- **ISO 27001:2022 Control:** Annex A 5.15 (Access Control) & Annex A 5.17 (Authentication Information). 

