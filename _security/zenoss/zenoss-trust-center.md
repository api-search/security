---
certifications:
- SOC 2 Type II
- CSA STAR Registry
description: Trust center for Zenoss, published by Virtana (which acquired Zenoss in May 2025) at virtana.com/trust. It is a single narrative page rather than a hosted trust portal — there is no document request portal, no subprocessor list, and no downloadable evidence pack — but it names specific attestations and describes data residency, retention and access controls.
kind: trust-center
layout: security
name: Zenoss Trust Center
name_suffix: Trust Center
overview: Zenoss maintains a public trust center documenting SOC 2 Type II and CSA STAR Registry compliance.
provider_name: Zenoss
provider_slug: zenoss
slug: zenoss-trust-center
source_filename: zenoss-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.virtana.com/trust/\nprovider: Zenoss\nproviderId: zenoss\ndescription: >-\n  Trust center for Zenoss, published by Virtana (which acquired Zenoss in May 2025) at\n  virtana.com/trust. It is a single narrative page rather than a hosted trust portal — there is no\n  document request portal, no subprocessor list, and no downloadable evidence pack — but it names\n  specific attestations and describes data residency, retention and access controls.\nurl: https://www.virtana.com/trust/\nhttp_status: 200\nportal_vendor: none (self-hosted page)\ncertifications:\n  - name: SOC 2 Type II\n    status: attested\n    evidence: '\"Virtana is SOC 2 Type II compliant. A copy of the report is available upon request.\"'\n    report_available: on request\n  - name: CSA STAR Registry\n    status: listed\n    evidence: >-\n      \"Our information security program is aligned with the CSA Cloud Controls Matrix, and we are\n      listed\
  \ on the STAR Registry.\"\ncompliance_programs:\n  - name: GDPR\n    evidence: '\"Virtana also maintains a privacy compliance program, which includes GDPR and CCPA.\"'\n  - name: CCPA\n    evidence: Named alongside GDPR in the same statement.\nnot_claimed:\n  - ISO/IEC 27001\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - ISO 27017 / 27018\ndata_residency:\n  infrastructure: AWS\n  model: >-\n    Clients choose the region that contains their data, and the data stays within that region.\n  regions:\n    - Europe — United Kingdom\n    - North America — United States Central\ndata_retention:\n  policy: >-\n    An active data retention policy retains or deletes data per applicable law. A departing customer\n    can access their data for up to 90 days unless otherwise requested; after 90 days Virtana\n    permanently deletes customer data.\n  customer_exit_window_days: 90\naccess_controls:\n  encryption: Industry-standard algorithms, encrypted in transit and at rest.\n  mfa: Multi-factor authentication\
  \ on all systems, for all access points, at all times.\n  logging: All data access is logged and monitored.\n  non_production_data: Development, test and QA data is anonymized and sanitized.\n  pen_testing: Penetration testing is performed against sanitized non-production environments.\nsso:\n  protocols:\n    - LDAP\n    - SAML\n    - OIDC\n  note: Supports external identity providers with redirect-back to the platform.\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No security.txt on any host, no /security or /vulnerability-disclosure page, no bug bounty\n    program on HackerOne, Bugcrowd or Intigriti, and no security@ contact published anywhere on\n    virtana.com, zenoss.com or the documentation. There is no way for an outside researcher to report\n    a vulnerability except the general Contact Us form. No Security pointer is emitted in apis.yml\n    because there is nothing to point at.\n  probes:\n    - url: https://www.virtana.com/.well-known/security.txt\n   \
  \   status: 404\n    - url: https://www.virtana.com/security.txt\n      status: 404\n    - url: https://docs.zenoss.io/.well-known/security.txt\n      status: 404\n    - url: https://api.virtana.ai/.well-known/security.txt\n      status: 404\n    - url: https://www.virtana.com/security/\n      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenoss/refs/heads/main/security/zenoss-trust-center.yml
summary_line: SOC 2 Type II, CSA STAR Registry
tags:
- AIOps
- Monitoring
- Observability
- Infrastructure
- Event Management
- Hybrid Cloud
- OpenTelemetry
- gRPC
- Metrics
trust_url: https://www.virtana.com/trust/
---
