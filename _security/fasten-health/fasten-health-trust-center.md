---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Fasten Connect API
  slug: fasten-connect
  spec_type: OpenAPI
  url: https://docs.connect.fastenhealth.com/api-reference/openapi.yaml
certifications:
- SOC 2
- HIPAA
description: ''
kind: trust-center
layout: security
name: Fasten Health Trust Center
name_suffix: Trust Center
overview: Fasten Health maintains a public trust center documenting SOC 2 and HIPAA compliance.
provider_name: Fasten Health
provider_slug: fasten-health
slug: fasten-health-trust-center
source_filename: fasten-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nprobe_result: >-\n  0-working/probe-security-programs.py returned \"trust=none\" for this provider. That is a false\n  negative caused by rendering, not an absence: trust.fastenhealth.com answers HTTP 200 with an\n  814-byte single-page-app shell that loads its content from\n  laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js, so the keyword check found\n  no trust/compliance terms in the served HTML. The certifications below are taken from the\n  company's own marketing site, which states them in server-rendered text.\nurl: https://trust.fastenhealth.com/\nplatform: Laika / Thoropass Trust Center\nhttp_status: 200\ncertifications:\n  - SOC 2\n  - HIPAA\ncommitments:\n  - {name: CARIN Alliance Code of Conduct, role: Signatory}\n  - {name: CMS Interoperability Framework, role: Pledged}\nagreements:\n  - {name: Business Associate Agreement (BAA), availability: Customers on upgraded plans}\n  - {name: Service\
  \ Level Agreement (SLA), availability: Customers on upgraded plans}\nclaims_verbatim:\n  - \"SOC2 & HIPAA-compliant — Enterprise-grade security\"\n  - \"SOC2 Certified\"\n  - \"Protected Health Information\"\n  - \"Carin Alliance Code of Conduct Signatory\"\nevidence:\n  - source: https://www.fastenhealth.com/\n    http_status: 200\n    kind: marketing-site-server-rendered-text\n    keywords: [SOC2 Certified, HIPAA-compliant, Protected Health Information, Carin Alliance Code of Conduct Signatory]\n  - source: https://www.fastenhealth.com/images/logos/thoropass-soc2.png\n    kind: auditor-badge\n    note: Thoropass SOC 2 badge referenced from the homepage.\n  - source: https://trust.fastenhealth.com/\n    http_status: 200\n    kind: trust-center\n    note: >-\n      JS-rendered Laika trust center. Reachable but machine-unreadable — the certification detail,\n      report request flow and subprocessor list are not in the served HTML.\n  - source: https://docs.connect.fastenhealth.com/support\n\
  \    http_status: 200\n    kind: docs\n    keywords: [Service Level Agreements, Business Associate Agreements]\npolicies:\n  terms_of_service: https://policy.fastenhealth.com/terms.html\n  privacy_policy: https://policy.fastenhealth.com/connect/privacy_policy.html\n  policy_repo: https://github.com/fastenhealth/policy\ngaps:\n  - No security.txt on any host (RFC 9116).\n  - No published vulnerability disclosure policy or bug bounty program found.\n  - >-\n    The trust center is a client-rendered SPA, so no certification, subprocessor or report metadata\n    is machine-readable; an agent or crawler evaluating Fasten's compliance posture sees nothing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fasten-health/refs/heads/main/security/fasten-health-trust-center.yml
summary_line: SOC 2, HIPAA
tags:
- Healthcare
- FHIR
- Personal Health Record
- Electronic Medical Record
- Health Data Interoperability
- TEFCA
- EHI Export
- Patient Consent
- Self-Hosted
- Open-Source
- HL7
- Healthcare Connectivity
trust_url: https://trust.fastenhealth.com/
---
