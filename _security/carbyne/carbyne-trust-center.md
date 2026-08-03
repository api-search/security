---
certifications:
- ISO/IEC 27001:2013
- ISO/IEC 27017
- SOC 2 Type II
- HIPAA / HITECH
- CSA STAR (CAIQ) Level 1
description: ''
kind: trust-center
layout: security
name: Carbyne Trust Center
name_suffix: Trust Center
overview: Carbyne maintains a public trust center documenting ISO/IEC 27001:2013, ISO/IEC 27017, SOC 2 Type II, HIPAA / HITECH, and CSA STAR (CAIQ) Level 1 compliance.
provider_name: Carbyne
provider_slug: carbyne
slug: carbyne-trust-center
source_filename: carbyne-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: https://carbyne.com/cloud-advantage/cloud-security/\nurl: https://carbyne.com/cloud-advantage/cloud-security/\nkind: security-and-compliance-page\nnote: Carbyne publishes no dedicated trust portal (trust.carbyne.com and carbyne.com/trust\n  both fail to resolve / 404). The Cloud Security page under Cloud Advantage is the\n  published security and compliance posture, naming certifications, controls and policy\n  areas. SOC 2 reports are request-only via a sales contact.\ncertifications:\n- name: ISO/IEC 27001:2013\n  scope: Information Security Management System covering infrastructure, datacenters\n    and services\n- name: ISO/IEC 27017\n  scope: Cloud-specific information security controls\n- name: SOC 2 Type II\n  scope: Audited annually by independent auditors; report available on request via\n    Carbyne sales contact\n  report_access: on-request\n- name: HIPAA / HITECH\n  scope: Safeguards for Protected Health\
  \ Information; Business Associate Agreements\n    available\n- name: CSA STAR (CAIQ) Level 1\n  scope: Cloud Security Alliance Consensus Assessments Initiative Questionnaire across\n    16 domains\nhosting:\n  provider: Amazon Web Services\n  government_cloud: AWS GovCloud\n  well_architected_review: true\ncontrols:\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS v1.2\n  password_storage: hashed and salted\n  mfa: true\n  rbac: true\n  sso: true\n  ids: OSSEC host-based intrusion detection\n  network: default deny-all cloud firewall; private subnets; per-customer VPC for single-tenant\n    deployments\n  endpoint: MDM + EDR with full-disk encryption on company workstations\nvulnerability_management:\n  application_security_testing: OWASP Top 10 tooling plus third-party review of design,\n    code and implementation\n  penetration_testing: periodic third-party pen tests in sandbox and production environments,\n    organized in consultation with customers\n  external_disclosure_program:\
  \ false\n  note: No public vulnerability disclosure policy, security.txt or bug bounty program\n    was found; see security/carbyne-vulnerability-disclosure absence recorded in well-known/carbyne-well-known.yml\nsecurity_policies:\n- Access Management\n- Change Management\n- Data Request\n- Data Management\n- Information Security\n- Incident Response\n- Policy Management and Maintenance\n- Risk Management\n- Vendor Management\n- Vulnerability Management\navailability:\n  uptime_claim: 99.999%\n  failover: multi-availability-zone and multi-region architecture\n  monitoring: 24/7 operations team with email and SMS alerting\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://carbyne.com/cloud-advantage/cloud-security/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbyne/refs/heads/main/security/carbyne-trust-center.yml
summary_line: ISO/IEC 27001:2013, ISO/IEC 27017, SOC 2 Type II, HIPAA / HITECH, CSA STAR (CAIQ) Level 1
tags:
- Company
- Emergency Services
- Public Safety
- Communications
- Telecommunications
- NG911
- Contact Center
- Location
- Video
- Government
- Artificial Intelligence
trust_url: https://carbyne.com/cloud-advantage/cloud-security/
---
