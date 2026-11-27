---
certification_count: 2
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Cloud Ex Machina Trust Center
name_suffix: Trust Center
overview: Cloud Ex Machina maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Cloud Ex Machina
provider_slug: cloudexmachina
slug: cloudexmachina-trust-center
source_filename: cloudexmachina-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://trust.cloudexmachina.io/\nurl: https://trust.cloudexmachina.io/\nhost: cloud-ex-machina.secureframetrust.com\nplatform: Secureframe Trust Center\ncertifications:\n- SOC 2\n- GDPR\ncertification_detail:\n- name: SOC 2 Type 2\n  status: achieved\n  verbatim: SOC 2 Type 2\n- name: ISO 27001\n  status: planned\n  target_year: 2026\n  verbatim: 'ISO 27001: Planned 2026.'\n- name: GDPR\n  status: addressed\n  verbatim: 'GDPR: Data Processing Addendum (DPA) available.'\nsubprocessors:\n- name: AWS\n  purpose: Cloud Provider\n- name: Google LLC\n  purpose: Google Cloud Platform\n  AI/ML services: null\n- name: Anthropic\n  purpose: AI/ML services\n- name: Nango\n  purpose: Product integrations\n- name: Sentry\n  purpose: Performance monitoring and error tracking\ncontrols_documented:\n- incident response\n- data retention and disposal\n- encryption and key management\n- vendor risk management\n- uptime and availability\
  \ monitoring\n- confidential reporting channel\ndisclosure:\n  policy_url: null\n  contact: null\n  bug_bounty: null\n  note: 'The trust center lists a \"Confidential Reporting Channel\" control — \"A confidential reporting\n    channel is made available to internal personnel and external parties to report security and other\n    identified concerns\" — but publishes no reachable policy URL, no security contact address in the served\n    HTML (contact addresses are rendered client-side and were not recoverable from the response body),\n    and no bug bounty program. /.well-known/security.txt returns 404 on www.cloudexmachina.io and a soft-200\n    HTML shell elsewhere; www.cloudexmachina.io/security returns 404. Because no disclosure channel could\n    be verified, NO VulnerabilityDisclosure or Security pointer is emitted in apis.yml. This is the single\n    clearest, cheapest improvement available to Cloud ex Machina: publish an RFC 9116 /.well-known/security.txt\n    naming a Contact\
  \ and a Policy.'\nevidence:\n- source: https://trust.cloudexmachina.io/\n  http_status: 200\n  keywords:\n  - soc 2\n  - iso 27001\n  - trust center\n  - gdpr\n  - subprocessor\n  - uptime\n- source: https://www.cloudexmachina.io/.well-known/security.txt\n  http_status: 404\n- source: https://www.cloudexmachina.io/security\n  http_status: 404\ncertifications_in_progress:\n- ISO 27001\ncertification_quotes:\n  ISO 27001: 'rds and are on track for formal certifications: | ISO 27001: Planned 2027.'\ncertifications_checked:\n  date: '2026-11-11'\n  by: probe-security-programs.classify_certs\n  note: a certification is listed only when the trust page states it as held (roadmap#1133)\n"
source_yaml_url: https://artifacts.apis.io/cloudexmachina/security/cloudexmachina-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- Company
- Infrastructure
- Cloud
- FinOps
- Cloud Cost Optimization
- Cloud Governance
- AI Agents
- Cloud Management
- Terraform
- Kubernetes
trust_url: https://trust.cloudexmachina.io/
---
