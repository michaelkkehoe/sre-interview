# Observability

## Monitoring concepts

*Q: What is white-box monitoring?*
A: White box monitoring is where you know the internals of the system. And the system has instrumentation in place to emit telemetry—metrics, logs, traces, etc (https://www.scalyr.com/blog/black-box-monitoring-track-opaque-systems/)

*Q: What is black-box monitoring?*
A: Black box monitoring is where you don’t have control and don’t know what’s happening inside the system. You only monitor the system from the outside—its behavior. (https://www.scalyr.com/blog/black-box-monitoring-track-opaque-systems/)_

*Q: What is the purpose of external monitoring?*
A: To ensure that your users can access your website (and that performance is acceptable). External monitoring helps detect CDN/ ISP issues.

*Q: What are some factors to consider with external monitoring?*
A: Cost (usually there is a cost to each test and/ or frequency). Ensuring that you do not DOS systems. 

*Q: Explain TTD, TTR and the importance of measuring it?*
A: 

* TTD: Time to detect
* TTR: Time to resolve
* Measuring these provide Key Performance Indicators (KPI) if your incident response is improving

## Distributed Tracing

*Q: What are the benefits of distributed tracing?*
A: You can get rich signals into where things are unhealthy in your system

*Q: What are some of the challenges with distributed tracing?*
A: Sampling, bias.

## Human-Ops

*Q: How to you detect alert fatigue?*
A: Report on how many alerts are firing for each team/ service

## Auto-remediation

*Q: Describe the pros of an auto-remediation system?*
A:

* Can be used to remediate live-sit incidents
* Can be used to perform automatic investigation during live-site incident

*Q: Describe the cons of an auto-remediation system?*
A:

* Can easily hide issues that get swept under the rug


*Q: What are the key features of an auto-remediation system?*
A:

* Ability to deploy
* Ability to auto-scale
* Ability to perform remote-execution
* Ability to query monitoring/ alerting sources

## Postmortems

*Q: What is the purpose of postmortems?*
A: Understand all contributing root causes, document the incident for future reference and pattern discovery, and enact effective preventative actions to reduce the likelihood or impact of recurrence.

*Q: How do you practice blameless postmortems?*
A: 

* Incident postmortems focused on growth – without the blame game. ...
* Communicate an open, mistake-friendly approach up front. ...
* Encourage honesty and acceptance of failure. ...
* Share information and build a timeline. ...
* Be consistently blameless. ...
* Get C-suite buy-in. ...
* Collaborate. ...
* Make decisions, but get approval.


*Q: What methods would you use to ensure postmortems are being held?*
A: 
