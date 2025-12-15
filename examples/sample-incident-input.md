## Incident Overview
- Incident ID: INC-2025-001
- Date & Time: 10-Dec-2025, 14:30 IST
- Severity: SEV1
- Services Impacted: Payment API

## Business Impact
- Checkout failures for 30% users
- Impact duration: 45 minutes

## Timeline
- Detected: 14:32
- Escalated: 14:35
- Mitigated: 15:05
- Resolved: 15:15

## Root Cause
- Expired TLS certificate on API gateway

## Resolution
- Certificate renewed and services restarted

## Lessons Learned
- Certificate monitoring was missing
