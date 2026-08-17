---
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Rallyware Trust Center
name_suffix: Trust Center
overview: Rallyware maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Rallyware
provider_slug: rallyware
slug: rallyware-trust-center
source_filename: rallyware-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://www.rallyware.com/security-2\nurl: https://www.rallyware.com/security-2\ntype: security posture page\ndedicated_trust_portal: false\nportal_note: >-\n  No trust.rallyware.com or security.rallyware.com exists (both fail to resolve,\n  probed 2026-08-14). What Rallyware publishes is a single narrative security page on\n  the marketing site — no document request flow, no downloadable report, no\n  subprocessor list, and no live control status.\n\ncertifications:\n- SOC 2\n- GDPR\n\ncertification_detail:\n- name: SOC 2\n  claim_text: >-\n    \"Our approach is based on the five SOC 2 Trust Service Criteria: security,\n    availability, processing integrity, confidentiality and privacy.\"\n  attestation_claimed: false\n  caveat: >-\n    Framed as the framework their approach is BASED ON. Rallyware does not claim a\n    completed Type I or Type II attestation, does not name an auditing firm, does not\n    state\
  \ a report period, and offers no path to request the report. Record as\n    published posture, not verified certification.\n- name: GDPR\n  claim_text: >-\n    No explicit GDPR compliance statement appears on the security page. The signal is\n    implementation-side: the site runs a GDPR cookie-consent implementation and\n    publishes a privacy policy, and the API data model carries a GDPR erasure marker\n    (UserProfile.deletion_requested_at) plus tenant-configurable privacy and cookie\n    policy pages.\n  attestation_claimed: false\n\nnot_claimed:\n- ISO 27001\n- ISO 27017\n- ISO 27018\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\n- FIPS 140\n\nprograms:\n- name: Information Security Management System (ISMS)\n  detail: Documented, updated annually, reviewed through internal and external audits.\n- name: Independent penetration testing\n  detail: Conducted annually.\n- name: Bug Bounty Program\n  detail: See security/rallyware-vulnerability-disclosure.yml.\n- name: Business continuity\
  \ / disaster recovery\n  detail: >-\n    BCP and DRP developed and regularly tested, covering pandemic, crisis\n    communication and disaster recovery scenarios.\n- name: Personnel security and training\n  detail: Security-culture and training program stated.\n\ninfrastructure:\n  cloud: AWS\n  detail: >-\n    \"Rallyware's infrastructure is built on AWS, following established security best\n    practices. Each service is designed and maintained with reliability and data\n    protection requirements in mind. Project environments are isolated.\"\n  corroboration: >-\n    Independently consistent with observed operations — the internal status page is\n    fronted by AWS Cognito (eu-central-1) and the public github.com/rallyware org\n    consists entirely of AWS Terraform modules (EKS, MWAA, SQS, Cognito, VPC, RDS).\n\nevidence:\n- source: https://www.rallyware.com/security-2\n  http_status: 200\n  keywords:\n  - soc 2\n  - gdpr\n  - isms\n  - penetration testing\n  - bug bounty\n  - business\
  \ continuity\n- source: https://trust.rallyware.com/\n  result: does not resolve\n- source: https://www.rallyware.com/security\n  http_status: 200\n  note: 302 redirect to /security-2, which is the canonical page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rallyware/refs/heads/main/security/rallyware-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- Company
- Sales Enablement
- Workforce Enablement
- Learning and Development
- Performance Management
- Gamification
- Direct Selling
- Enterprise Software
trust_url: https://www.rallyware.com/security-2
---
