## Enhancing Windows Security Monitoring: Firewall Exception Analysis





### Background:
As part of our ongoing efforts to improve our security posture and maintain compliance with industry standards, the SOC manager has identified a critical gap in our Windows activity monitoring.

#### Objective:

Implement real-time visibility into changes made to the Windows Firewall Exception List, with a specific focus on newly added rules. This enhancement will significantly improve our ability to detect and respond to potential security breaches and unauthorized changes to our network perimeter.

#### Action Items:
1. Extend the existing 'Windows Activity' dashboard in our SIEM platform to include a new panel dedicated to Windows Firewall Exception monitoring.
2. Develop and implement custom queries to track and display all new rules added to the Windows Firewall Exception List across our enterprise environment.
3. Set up automated alerts for any suspicious or unauthorized additions to the Firewall Exception List.
4. Create a weekly report summarizing all changes to the Firewall Exception List for management review.
<img width="468" alt="1 4946" src="https://github.com/user-attachments/assets/fdfd773f-5cab-4bb9-8082-5b66b298631f">

### Event ID Identification Research and confirm Event ID 4946 corresponds to Windows Firewall Exception List changes.

<img width="468" alt="2" src="https://github.com/user-attachments/assets/e79240ec-1d24-4911-a15f-8933c0b125fc">

### Splunk Query Execution Search Splunk for Event ID 4946 in Verbose Mode. Verify the presence of relevant events.
<img width="468" alt="3" src="https://github.com/user-attachments/assets/944a2eab-382c-4030-a734-25e891b1571f">

### Event Field Analysis Examine the top event to identify key fields: Computer, Profile Changed, Rule Name, and Rule ID.
<img width="468" alt="4" src="https://github.com/user-attachments/assets/85183900-42b2-44f9-a5d2-24ea35cb4a75">

### Query Optimization Develop a transformation command using 'stats' with the identified fields and _time. Include 'sort +_time' for chronological ordering.
<img width="468" alt="5" src="https://github.com/user-attachments/assets/a9aaa60c-805f-4f2d-a4b6-813167be62ec">

### Dashboard Enhancement Integrate the new query into the existing 'Windows Activity' dashboard. Create a new panel titled 'Firewall Exception Added'.

<img width="397" alt="6" src="https://github.com/user-attachments/assets/f0b1771a-44e4-4917-a4f1-3f78d7be053c">

By implementing this enhancement, we will significantly strengthen our ability to protect critical assets and maintain a robust security perimeter in our Windows environment.

