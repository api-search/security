---
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Artillery Trust Center
name_suffix: Trust Center
overview: Artillery maintains a public trust center covering its security and compliance posture.
provider_name: Artillery
provider_slug: artillery
slug: artillery-trust-center
source_filename: artillery-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nprobe: true\nsource: https://www.artillery.io/docs/resources/security\nurl: https://www.artillery.io/docs/resources/security\ntrust_center: false\nnote: >-\n  Artillery runs NO trust center. trust.artillery.io does not resolve and security.artillery.io\n  was not found; probe-security-programs.py returned trust=none. What Artillery does publish is\n  a \"Security Overview\" documentation page describing its own posture, plus a Security Policy\n  under Legal & Compliance. It names NO third-party certification — no SOC 2, ISO 27001, PCI\n  DSS, HIPAA or FedRAMP claim appears anywhere on the site. This file records the posture page\n  and the ABSENCE of certifications; no Compliance pointer is emitted, because there is no\n  published compliance program to point at.\ncertifications: []\nbenchmarks_self_asserted:\n- name: AWS Foundational Security Best Practices\n  version: 1.0.0\n  method: continuous verification via AWS Audit Manager\
  \ and Security Hub\n- name: CIS AWS Foundations Benchmark\n  version: 1.2.0\n  method: continuous verification via AWS Audit Manager and Security Hub\nposture_claims:\n- MFA and single sign-on enforced across all services\n- CI/CD with protected main/deployment branches\n- static security analysis and dependency scanning with automated alerting\n- centralized logging for auditing and alerting\n- infrastructure as code, all changes through CI/CD\n- AWS assume-role access with CloudTrail auditing\n- MDM endpoint security on all employee and contractor devices\n- regular third-party pentests of Artillery Cloud\n- encryption at rest for all Artillery Cloud data\n- AWS account, VPC and security group segmentation\n- 'self-hosted CLI by design: Artillery staff have no access to test scripts, targets, credentials or test data'\ndata_residency:\n  byoc: true\n  note: >-\n    \"Deploy to your own AWS account (BYOC)\" is offered on the pricing page for companies whose\n    compliance policies require\
  \ data to remain in their own cloud; contact sales@artillery.io.\nevidence:\n- source: https://www.artillery.io/docs/resources/security\n  http_status: 200\n  keywords: [supply chain security, security best-practices, pentests, encryption at rest, vendor security]\n- source: https://trust.artillery.io\n  http_status: 0\n  result: DNS does not resolve\n- source: https://www.artillery.io/trust\n  http_status: 404\nx-evidence:\n  fetched: '2026-09-07'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artillery/refs/heads/main/security/artillery-trust-center.yml
summary_line: trust center published
tags:
- Load Testing
- Performance Testing
- Open-Source
- Testing
- DevOps
- Node.js
trust_url: https://www.artillery.io/docs/resources/security
---
