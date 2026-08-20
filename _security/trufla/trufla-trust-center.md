---
certifications: []
description: ''
kind: trust-center
layout: security
name: Trufla Trust Center
name_suffix: Trust Center
overview: Trufla maintains a public trust center covering its security and compliance posture.
provider_name: Trufla
provider_slug: trufla
slug: trufla-trust-center
source_filename: trufla-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nsource: https://trust.trufla.com/\nurl: https://trust.trufla.com/\nplatform: SafeBase\ndns: CNAME trufla.portals.safebase.io\nhttp_note: Returns 403 to non-browser clients (Cloudflare); renders for a normal\n  browser user agent.\ncertifications: []\ncertification_status: >-\n  None published. The trust center states \"We are working towards compliance\n  certifications\" and \"We are working on our security compliance\" — no SOC 2,\n  ISO 27001, PCI DSS, HIPAA, FedRAMP, CSA STAR or FIPS certification is named as\n  completed. No Compliance pointer is wired in apis.yml as a result.\nsubprocessors:\n- name: Amazon Web Services\n  role: infrastructure provider\ndocuments_available_on_request:\n- security reports\n- completed security questionnaires / self-assessments\n- risk mitigation and recovery objectives\n- data security practices\n- access control practices\n- infrastructure provider detail\n- endpoint security\n-\
  \ incident response procedures\n- risk management\n- continuous monitoring\naccess: Gated — documents are released through a \"Get access\" / \"Ask for\n  information\" request flow rather than published openly.\nevidence:\n- source: https://trust.trufla.com/\n  keywords:\n  - trust center\n  - compliance certification\n  - subprocessors\n  - incident response\nrelated:\n  vulnerability_disclosure: none published — /.well-known/security.txt returns\n    404 and no bug bounty or responsible-disclosure page exists\n  domain_security: security/trufla-domain-security.yml\n  privacy_policy: https://www.trufla.com/legal/privacy-policy/\n  acceptable_use_policy: https://www.trufla.com/legal/acceptable-use-policy/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trufla/refs/heads/main/security/trufla-trust-center.yml
summary_line: trust center published
tags:
- Insurance
- Canada
- Property and Casualty
- Insurtech
- Brokers
- Agency Management
- CSIO
- Policy Administration
- Quote Bind Issue
- Digital Distribution
trust_url: https://trust.trufla.com/
---
