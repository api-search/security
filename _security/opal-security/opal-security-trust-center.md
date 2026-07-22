---
api_specs:
- filename: opal-security-openapi.yaml
  format: yaml
  label: Opal API
  slug: opal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal-security/refs/heads/main/openapi/opal-security-openapi.yaml
certifications: []
description: ''
kind: trust-center
layout: security
name: Opal Security Trust Center
name_suffix: Trust Center
overview: Opal Security maintains a public trust center covering its security and compliance posture.
provider_name: Opal Security
provider_slug: opal-security
slug: opal-security-trust-center
source_filename: opal-security-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://opal.dev/security\nprovider: Opal Security\nlegal_entity: Perma Security, Inc. (dba Opal)\ntrust_center:\n  url: https://opal.dev/security\n  name: Trust Center\n  last_updated: '2025-06-05'\ncompliance:\n- name: SOC 2\n  status: documented\n  detail: >-\n    The Trust Center describes SOC 2 as the auditing procedure Opal follows;\n    an independent third-party penetration test is performed at least annually.\n- name: GDPR\n  status: documented\n- name: CCPA\n  status: documented\nsecurity_measures:\n- Personnel security awareness training and confidentiality agreements.\n- Two-factor authentication gating production data access; time-bound, on-call event-bound elevated access; periodic access reviews.\n- Encryption in transit (TLS 1.2+ / VPN) and at rest (AWS KMS), including database backups.\n- Automated alerting and searchable audit logging of access-change events; internal Opal employee actions logged.\n- Daily\
  \ encrypted database backups (AWS KMS) for the cloud offering.\n- Secure SDLC — third-party automated security testing pre-release, peer-reviewed production releases.\n- Intrusion prevention/detection monitoring; documented incident response plan.\n- Vulnerability management program with monthly internal scans and >= annual third-party penetration testing.\nsubprocessors:\n- name: Amazon Web Services (AWS)\n  purpose: Hosting and cloud infrastructure\n  region: USA\n- name: Auth0\n  purpose: Developer user identity platform\n  region: USA\n- name: LaunchDarkly\n  purpose: Feature release management\n  region: USA\n- name: Anthropic\n  purpose: LLM API for remediation recommendations, request feedback, taxonomy suggestions\n  region: USA\ncontacts:\n  security: security@opal.dev\n  subprocessors: subprocessors@opal.dev\ndocuments:\n  privacy_policy: https://opal.dev/privacy-policy\n  terms_of_service: https://opal.dev/terms-of-service\n  saas_agreement: https://opal.dev/saas-agreement\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opal-security/refs/heads/main/security/opal-security-trust-center.yml
summary_line: trust center published
tags:
- Company
- Cybersecurity
- Access Management
- Identity and Access Management
- Least Privilege
- Access Reviews
- Security
trust_url: ''
---
