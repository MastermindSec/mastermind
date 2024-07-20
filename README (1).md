
# Hi, I'm Katherine! 👋


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

### Event ID Identification Research and confirm Event ID 4946 corresponds to Windows Firewall Exception List changes.

### Splunk Query Execution Search Splunk for Event ID 4946 in Verbose Mode. Verify the presence of relevant events.

### Event Field Analysis Examine the top event to identify key fields: Computer, Profile Changed, Rule Name, and Rule ID.

### Query Optimization Develop a transformation command using 'stats' with the identified fields and _time. Include 'sort +_time' for chronological ordering.

### Dashboard Enhancement Integrate the new query into the existing 'Windows Activity' dashboard. Create a new panel titled 'Firewall Exception Added'.