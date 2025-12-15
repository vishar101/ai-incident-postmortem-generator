## Executive Summary
On 10-Dec-2025, a SEV1 incident impacted the Payment API, causing checkout failures for approximately 30% of users for 45 minutes. The issue was caused by an expired TLS certificate on the API gateway. The incident was detected quickly and mitigated within 35 minutes. Services were fully restored after certificate renewal. Preventive measures have been identified to avoid recurrence.

## Root Cause Analysis (5 Whys)
1. Why did the API fail?  
   → TLS handshake failures occurred.
2. Why did TLS fail?  
   → The certificate had expired.
3. Why was it expired?  
   → No automated renewal process was configured.
4. Why was automation missing?  
   → Certificate lifecycle was not part of monitoring scope.
5. Why was it excluded?  
   → Ownership and review process were unclear.

## Preventive Actions
- Implement automated certificate renewal
- Add certificate expiry alerts
- Quarterly operational readiness reviews

## Customer Communication
We experienced a temporary disruption due to a security certificate issue, which has now been fully resolved. Our teams have implemented additional monitoring to prevent this from happening again.
