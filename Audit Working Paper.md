# **Audit Working Paper** 

## **Objective** 

To verify that compromised accounts had their active sessions and OAuth tokens revoked within the mandated 30-minute period defined in the Access Control Policy. 

## **Scope** 

Review of Google Workspace administrator audit logs for 4 reported phishing incidents in August 2026. 

## **Methodology** 

Extracted ‘Session Terminate’ and ‘Password Reset’ timestamps from the Google Workspace Admin Console and compared them against the initial reported incident time. 

## **Evidence Testing Table** 

|Incident ID|Afected<br>User|Incident<br>Reported<br>Time|Sessions<br>Revoked<br>Time|Time<br>Elapsed|SLA Met<br>(Pass/Fail)?|
|---|---|---|---|---|---|
|INC-001|J.Doe|09:00 AM|09:17 AM|17 mins|PASS|
|INC-002|M.Smith|12:20 PM|12:35 PM|15 mins|PASS|
|INC-003|A.Wong|03:00 PM|03:10 PM|10 mins|PASS|
|INC-004|R.Patel|04:30 PM|05:24 PM|54 mins|FAIL (Non-<br>Conformity)|



## **Findings & Corrective Action** 

- Finding: 1 out of 4 incidents failed the 30-minute SLA (INC-004). 

- Root Cause: The IT administrator was away from their workspace and missed the alert. 

- Corrective Action (CAPA): Configure an automated script in the SIEM/SOAR platform to automatically revoke Google Workspace sessions upon high-severity phishing alerts, removing the reliance on manual IT intervention. 

