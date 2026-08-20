---
certifications:
- SOC 2 Type 2
- GDPR
- EU-US Privacy Shield
- Penetration testing
description: ''
kind: trust-center
layout: security
name: Hull Trust Center
name_suffix: Trust Center
overview: Hull maintains a public trust center documenting SOC 2 Type 2, GDPR, EU-US Privacy Shield, and Penetration testing compliance.
provider_name: Hull
provider_slug: hull
slug: hull-trust-center
source_filename: hull-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.hull.io/security/\nkind: security-and-compliance-page\nnote: >-\n  Hull publishes no dedicated trust centre (no trust.hull.io, no Vanta/Drata/\n  SafeBase portal — all probed 404 on 2026-08-13). Its compliance posture is\n  stated on a single narrative /security/ page plus an \"Enterprise features\" row\n  in the pricing table. Attestations are named but no report, audit window,\n  auditor or certificate is published; every artifact is gated behind an email\n  request to security@hull.io.\ncertifications:\n  - name: SOC 2 Type 2\n    status: claimed\n    evidence: >-\n      Listed as an \"Enterprise features\" row on https://www.hull.io/pricing/,\n      marked Available on the Team, Business and Business + tiers.\n    report_available: on request\n  - name: GDPR\n    status: claimed\n    evidence: >-\n      \"Hull is committed to compliance with the General Data Protection\n      Regulation (GDPR)… Please\
  \ also get in touch to receive our Data Processing\n      Agreement (DPA) from security@hull.io.\"\n    report_available: DPA on request\n  - name: EU-US Privacy Shield\n    status: claimed\n    evidence: >-\n      \"Privacy Shield Compliant\" row on the pricing page. Note that the\n      Privacy Shield framework was invalidated by Schrems II in July 2020; the\n      claim predates that and was never updated.\n    report_available: false\n  - name: Penetration testing\n    status: claimed\n    evidence: >-\n      \"The Hull Platform undergoes regular penetration testing by independent\n      third parties… To get a copy of our test results please send inquiry to\n      security@hull.io.\"\n    report_available: on request\ninherited_certifications:\n  - provider: Amazon Web Services\n    note: >-\n      \"Hull utilizes Amazon Web Services for our platform infrastructure. Our\n      customers also benefit from Amazon Web Services Cloud Compliance security\n      and privacy measures including\
  \ ISO and SOC certifications.\"\n  - provider: Heroku, Elastic and other sub-processors\n    note: >-\n      \"our partners maintain but not limited to a SOC2 compliance and ISO\n      certification listed on their websites.\" These are the sub-processors'\n      certifications, not Hull's.\ndata_handling:\n  hosting: Amazon Web Services\n  headquarters: Atlanta, GA, United States\n  offices: [Atlanta GA (HQ), Paris France]\n  international_transfers: >-\n    \"We may transfer personal data outside of the country it was collected in or\n    outside of the European Economic Area (EEA)… we comply with the applicable\n    legal requirements of providing adequate safeguards.\"\n  backups: [platform automatic back-ups, infrastructure replication, workflow/business-logic snapshots]\n  on_call: Global on-call engineering rotation documented.\ncontact: security@hull.io\nprivacy_policy: https://www.hull.io/pp/\nevidence:\n  - source: https://www.hull.io/security/\n    http_status: 200\n    fetched:\
  \ '2026-08-13'\n    keywords: [GDPR, SOC2, ISO, penetration testing, Data Processing Agreement, security@hull.io]\n  - source: https://www.hull.io/pricing/\n    http_status: 200\n    fetched: '2026-08-13'\n    keywords: [GDPR Compliant, Privacy Shield Compliant, SOC2 Type 2, Penetration Testing]\n  - source: https://trust.hull.io/\n    http_status: 000\n    fetched: '2026-08-13'\n    note: Host does not resolve.\n  - source: https://www.hull.io/trust/\n    http_status: 404\n    fetched: '2026-08-13'\n  - source: https://www.hull.io/compliance/\n    http_status: 404\n    fetched: '2026-08-13'\ncaveat: >-\n  Hull was shut down on 2022-12-31 and all infrastructure decommissioned; these\n  compliance claims describe a platform that no longer processes data. The\n  /security/ page also fails TLS verification (see\n  security/hull-domain-security.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hull/refs/heads/main/security/hull-trust-center.yml
summary_line: SOC 2 Type 2, GDPR, EU-US Privacy Shield, Penetration testing
tags:
- Company
- Customer Data Platform
- CDP
- Identity Resolution
- Data Integration
- Customer Data
- Marketing
- Real-Time
- iPaaS
- Analytics
trust_url: https://www.hull.io/security/
---
