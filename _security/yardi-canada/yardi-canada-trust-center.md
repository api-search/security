---
api_specs:
- filename: yardi-canada-status-openapi.yml
  format: yaml
  label: Yardi Systems Status API
  slug: yardi-systems-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-status-openapi.yml
certifications:
- SOC 2 (annual)
- SOC 1 (biannual)
- SSAE 18
- PCI
- HIPAA
- Sarbanes-Oxley
- CSA STAR Level 2
- FIPS 140-2 (key management)
description: ''
kind: trust-center
layout: security
name: Yardi Canada Trust Center
name_suffix: Trust Center
overview: Yardi Canada maintains a public trust center documenting SOC 2 (annual), SOC 1 (biannual), SSAE 18, PCI, HIPAA, Sarbanes-Oxley, CSA STAR Level 2, and FIPS 140-2 (key management) compliance.
provider_name: Yardi Canada
provider_slug: yardi-canada
slug: yardi-canada-trust-center
source_filename: yardi-canada-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nprobe: false\nurl: https://www.yardi.com/company/cloud-security/\nname: Yardi Cloud Security\nsummary: >-\n  Yardi has no branded trust portal — trust.yardi.com does not resolve and\n  /trust, /security and /compliance all 404 on www.yardi.com, which is why the\n  automated trust-centre probe recorded nothing. What it does have is a single\n  substantive Cloud Security page, reachable only through the company sitemap, that\n  names real certifications and audit cadences. That page is the trust surface, and it\n  is recorded here because the certifications on it are specific and checkable rather\n  than marketing adjectives.\ncertifications:\n  - SOC 2 (annual)\n  - SOC 1 (biannual)\n  - SSAE 18\n  - PCI\n  - HIPAA\n  - Sarbanes-Oxley\n  - CSA STAR Level 2\n  - FIPS 140-2 (key management)\ncontrols:\n  encryption_in_transit: Automatic TLS encryption with active session management; encrypted cookies validated against the database before\
  \ each request.\n  encryption_at_rest: Optional AES-256 database encryption available on request; keys managed in a FIPS 140-2 compliant system.\n  access_control: SSO integration, granular multi-level user/group privileges, administrator-set password complexity and expiration, automated inactivity log-off.\n  network: Intrusion Prevention Systems (IPS) and multiple firewalls.\n  testing: Third-party penetration tests and audits by external security vendors, described as regular and ongoing.\n  physical: 15 global data centres with 24/7 server-operations monitoring, biometric screening, video surveillance and on-premises personnel.\n  monitoring: 24/7 system monitoring, disaster recovery.\nevidence:\n  - source: https://www.yardi.com/company/cloud-security/\n    status: 200\n    keywords: [PCI, SSAE 18, Sarbanes-Oxley, HIPAA, SOC2, SOC1, CSA Star Level 2, FIPS140-2, AES256, penetration tests]\n    quote: >-\n      \"Feel confident your Cloud solution complies with PCI, SSAE 18 and Sarbanes-Oxley\n\
  \      regulations. Senior Living providers can rest assured with resident health data\n      adhering to the latest HIPAA rules. Annual SOC2 and biannual SOC1 reports are\n      provided to ensure compliance with SSAE18 and other accounting standards. The\n      Yardi Coud is CSA Star Level 2 certified by the Cloud Security Alliance.\"\nmisses:\n  - {url: 'https://trust.yardi.com/', status: 000, note: does not resolve}\n  - {url: 'https://www.yardi.com/trust/', status: 404}\n  - {url: 'https://www.yardi.com/security/', status: 404}\n  - {url: 'https://www.yardi.com/company/security/', status: 404}\n  - {url: 'https://www.yardi.com/security-and-compliance/', status: 404}\ngaps:\n  - No report request/download portal; SOC 1 and SOC 2 reports are described as \"provided\" but no request path is published.\n  - No vulnerability disclosure policy, bug bounty or security.txt anywhere on the estate (see security/yardi-canada-vulnerability-disclosure — none found).\n  - No Canadian data-residency\
  \ statement, despite Voyager, Breeze, Elevate, Investor Portal, Resident Screening and EHR Interfaces each running an explicit Canada region on the status page.\n  - No sub-processor list on the security page; a sub-processor page exists separately at https://www.yardi.com/about-us/legal/yardi-sub-processors.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/security/yardi-canada-trust-center.yml
summary_line: SOC 2 (annual), SOC 1 (biannual), SSAE 18, PCI, HIPAA, Sarbanes-Oxley, CSA STAR Level 2, FIPS 140-2 (key management)
tags:
- Real Estate
- Canada
- Property Management
- Rentals
- Commercial Real Estate
- PropTech
- Multifamily
- Affordable Housing
- Senior Living
- Investment Management
- Tenancy
- Payments
- MCP
- AI
trust_url: https://www.yardi.com/company/cloud-security/
---
