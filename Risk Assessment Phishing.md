# **Risk Assessment: Phishing** 

## **Roles & Responsibilities** 

Applies to: 

- All employees, contractors, third-party users using company resources 

- SOC Analyst 

- IT System Administrator 

- GRC Analyst 

- Information Security Manager 

## **Definitions** 

- Likelihood: 1 (Low), 2 (Medium), 3 (High) 

- Impact: 1 (Minor), 2 (Moderate), 3 (Severe) 

- Overall risk rating: Likelihood × Impact 

   - 1 – 2: Low Risk (Green) 

   - 3 – 4: Medium Risk (Yellow) 

   - 6 – 9: High Risk (Red) 

## **Risk Register** 

|Ris<br>k ID|Risk<br>Description|Inherent<br>Likelihoo<br>d|Inherent<br>Impact|Inhere<br>nt<br>Rating|Controls|Residual<br>Likelihoo<br>d|Residual<br>Impact|Residu<br>al<br>Rating|
|---|---|---|---|---|---|---|---|---|
|R-0<br>01|Employee<br>enters<br>credentials<br>into a cloned<br>phishing<br>site, leading<br>to<br>unauthorize<br>d account<br>access.|3 (High)|3<br>(Severe)|9<br>(High)|MFA and<br>Geographic<br>Anomaly<br>Alerts|1 (Low)|2<br>(Moderat<br>e)|2 (Low)|
|R-0<br>02|Threat actor<br>creates<br>covert email<br>auto-<br>forwarding<br>rules to<br>exfltrate<br>sensitive<br>internal<br>emails.|2<br>(Medium<br>)|3<br>(Severe)|6<br>(High)|Immediate<br>inspection<br>and<br>removal of<br>unauthorize<br>d inbox<br>rules during<br>incident.|1 (Low)|2<br>(Moderat<br>e)|2 (Low)|
|R-0<br>03|Compromis<br>ed user<br>account<br>accesses<br>internal|2<br>(Medium<br>)|3<br>(Severe)|6<br>(High)|30-day<br>lookback<br>audit log<br>review and<br>principle of|1 (Low)|2<br>(Moderat<br>e)|2 (Low)|



||shared<br>drives<br>containing<br>customer<br>data.||||least<br>privilege.||||
|---|---|---|---|---|---|---|---|---|
|R-0<br>04|Delayed<br>session<br>revocation<br>allows threat<br>actor to<br>maintain<br>persistent<br>access after<br>password<br>reset.|3 (High)|2<br>(Moderat<br>e)|6<br>(High)|Revocation<br>of session<br>and OAuth<br>token<br>within 30<br>minutes.|1 (Low)|1 (Low)|1 (Low)|



## **Risk-Based Decision** 

- All identified inherent high risks have been reduced to acceptable residual level (Low). 

- Remaining residual risk is subject to Information Security Manager’s decision. 

- Annual review and continuous log monitoring are highly recommended. 

