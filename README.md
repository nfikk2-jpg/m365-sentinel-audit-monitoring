# Microsoft Sentinel — Microsoft 365 Audit Monitoring & Detection

## Project Overview

Designed, implemented, and validated a Microsoft 365 security monitoring solution using Microsoft Sentinel, Microsoft Purview, Azure Log Analytics, and Kusto Query Language (KQL).

The project demonstrates end-to-end audit collection, security event investigation, scheduled detection, and incident response.

## Technologies Used

- Microsoft Sentinel
- Microsoft Defender
- Microsoft Purview Audit
- Microsoft 365 / OneDrive / SharePoint
- Azure Log Analytics
- Kusto Query Language (KQL)

## Implementation

1. Configured Microsoft 365 audit log ingestion into Microsoft Sentinel.
2. Generated controlled OneDrive file access, modification, and rename activity.
3. Investigated security events using KQL queries against the `OfficeActivity` table.
4. Developed and validated a file rename detection query.
5. Deployed an hourly scheduled analytics rule.
6. Confirmed successful security alert and incident generation.
7. Resolved the test incident and disabled the demonstration rule.

## Results

| Validation | Result |
|---|---|
| Purview audit records | 256 retrieved |
| Sentinel event ingestion | 112 records initially verified |
| OneDrive document investigation | 7 matching events |
| File rename detection | Successful |
| Scheduled analytics rule | Deployed and tested |
| Security incident | ID 1 generated |
| Incident resolution | Completed |
| Post-test cleanup | Detection rule disabled |

## Security Engineering Considerations

File-renaming activity alone is not evidence of malicious behavior. This controlled demonstration used informational severity to validate the monitoring and alerting workflow.

A production deployment would require additional behavioral conditions, entity mapping, tuning, and false-positive reduction.

## Project Outcome

Successfully demonstrated Microsoft 365 security telemetry flowing into Microsoft Sentinel, KQL-based investigation, scheduled analytics detection, and automated incident generation.

**Environment:** Microsoft 365 E5 evaluation and Microsoft Sentinel test workspace.

**Focus:** Cloud Security Engineering, Security Monitoring, Detection Engineering, and Incident Investigation.
