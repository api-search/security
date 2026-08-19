---
certifications:
- SOC 2
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Cloudexmachina Trust Center
name_suffix: Trust Center
overview: Cloud Ex Machina maintains a public trust center documenting SOC 2, ISO 27001, and GDPR compliance.
provider_name: Cloud Ex Machina
provider_slug: cloudexmachina
slug: cloudexmachina-trust-center
source_filename: cloudexmachina-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://trust.cloudexmachina.io/\nurl: https://trust.cloudexmachina.io/\nhost: cloud-ex-machina.secureframetrust.com\nplatform: Secureframe Trust Center\ncertifications:\n- SOC 2\n- ISO 27001\n- GDPR\ncertification_detail:\n- {name: SOC 2 Type 2, status: achieved, verbatim: 'SOC 2 Type 2'}\n- {name: ISO 27001, status: planned, target_year: 2026, verbatim: 'ISO 27001: Planned 2026.'}\n- {name: GDPR, status: addressed, verbatim: 'GDPR: Data Processing Addendum (DPA) available.'}\nsubprocessors:\n- {name: AWS, purpose: Cloud Provider}\n- {name: Google LLC, purpose: Google Cloud Platform, AI/ML services}\n- {name: Anthropic, purpose: AI/ML services}\n- {name: Nango, purpose: Product integrations}\n- {name: Sentry, purpose: Performance monitoring and error tracking}\ncontrols_documented:\n- incident response\n- data retention and disposal\n- encryption and key management\n- vendor risk management\n- uptime and availability\
  \ monitoring\n- confidential reporting channel\ndisclosure:\n  policy_url: null\n  contact: null\n  bug_bounty: null\n  note: >-\n    The trust center lists a \"Confidential Reporting Channel\" control — \"A confidential reporting\n    channel is made available to internal personnel and external parties to report security and\n    other identified concerns\" — but publishes no reachable policy URL, no security contact address\n    in the served HTML (contact addresses are rendered client-side and were not recoverable from\n    the response body), and no bug bounty program. /.well-known/security.txt returns 404 on\n    www.cloudexmachina.io and a soft-200 HTML shell elsewhere; www.cloudexmachina.io/security\n    returns 404. Because no disclosure channel could be verified, NO VulnerabilityDisclosure or\n    Security pointer is emitted in apis.yml. This is the single clearest, cheapest improvement\n    available to Cloud ex Machina: publish an RFC 9116 /.well-known/security.txt naming a\
  \ Contact\n    and a Policy.\nevidence:\n- source: https://trust.cloudexmachina.io/\n  http_status: 200\n  keywords: [soc 2, iso 27001, trust center, gdpr, subprocessor, uptime]\n- source: https://www.cloudexmachina.io/.well-known/security.txt\n  http_status: 404\n- source: https://www.cloudexmachina.io/security\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudexmachina/refs/heads/main/security/cloudexmachina-trust-center.yml
summary_line: SOC 2, ISO 27001, GDPR
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
