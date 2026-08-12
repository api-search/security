---
certifications:
- SOC 2 Type I
description: ''
kind: trust-center
layout: security
name: Buildops Trust Center
name_suffix: Trust Center
overview: BuildOps maintains a public trust center documenting SOC 2 Type I compliance.
provider_name: BuildOps
provider_slug: buildops
slug: buildops-trust-center
source_filename: buildops-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nprobe: true\nurl: https://trust.buildops.com/\nplatform: Vanta\ncertifications:\n- SOC 2 Type I\nattestations:\n- name: Penetration test certificate\n  issuer: Astra (https://www.getastra.com/)\n  note: BuildOps' security policy states penetration testing is performed annually\n    by an independent assessor.\nreports:\n- name: BuildOps SOC 2 Type I Certificate\n  access: request via trust center\npolicies_listed:\n- Human Resource Security Policy\n- Access Control Policy\n- Business Continuity and Disaster Recovery Plan\n- Data Management Policy\n- Incident Response Plan\ncontrol_families:\n- {name: Infrastructure security, controls_listed: 11}\n- {name: Organizational security, controls_listed: 11}\n- {name: Product security, controls_listed: 4}\n- {name: Internal security procedures, controls_listed: 31}\n- {name: Data and privacy, controls_listed: 3}\nsubprocessors:\n- {name: Amazon Web Services, role: Cloud provider, region: United\
  \ States}\n- {name: Okta, role: Identity Provider, region: United States}\n- {name: Payabli, role: Finance and Payments, region: United States}\n- {name: Snowflake, role: Data storage and processing, region: United States}\ncontact: security@buildops.com\nsecurity_policy: https://buildops.com/security-policy\nevidence:\n- source: https://trust.buildops.com/\n  http_status: 200\n  keywords: [trust center, compliance, soc 2 type i, penetration testing, controls,\n    subprocessors]\n  note: >-\n    The trust center is a Vanta client-side application; the served HTML is a\n    shell. Contents captured by rendering the page, not by reading the raw HTML.\n    This is why the standard keyword probe (probe-security-programs.py) records\n    no hit against it.\n- source: https://buildops.com/security-policy\n  http_status: 200\n  keywords: [soc 2 type i, encryption, multi-factor authentication, penetration testing,\n    incident response]\ngaps:\n- SOC 2 Type I only; no Type II, ISO 27001, PCI\
  \ DSS, HIPAA or FedRAMP named.\n- No public status page. The status widget embedded in the Dev Center belongs to\n  Stoplight (kmmfkblgkhnf.statuspage.io = \"Stoplight\"), not to BuildOps.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildops/refs/heads/main/security/buildops-trust-center.yml
summary_line: SOC 2 Type I
tags:
- Company
- Construction Software
- Field Service Management
- Contractor Management
- Commercial Services
- HVAC
- ERP Integration
- CRM
trust_url: https://trust.buildops.com/
---
