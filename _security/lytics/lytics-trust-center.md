---
api_specs:
- filename: lytics-api-v2-openapi.json
  format: json
  label: Lytics API v2
  slug: lytics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-api-v2-openapi.json
- filename: lytics-api-v1-openapi.json
  format: json
  label: V1 Lytics API
  slug: lytics-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-api-v1-openapi.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Lytics Trust Center
name_suffix: Trust Center
overview: Lytics maintains a public trust center covering its security and compliance posture.
provider_name: Lytics
provider_slug: lytics
slug: lytics-trust-center
source_filename: lytics-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.lytics.com/\nredirects_to: https://trust.contentstack.com/\ncertifications: []\nnote: >-\n  Lytics publishes a trust center and names it in its own documentation —\n  https://docs.lytics.com/docs/consent says \"For more information on Lytics' security\n  and privacy program, please visit Lytics' trust center at https://trust.lytics.com/\".\n  Probed 2026-08-13: trust.lytics.com returns HTTP 200 and 302-redirects to\n  trust.contentstack.com, which is legitimate — Lytics joined Contentstack in January\n  2025 and the group trust center now serves both brands. The page is a Next.js\n  application that renders entirely client-side: the served HTML is a 12KB shell with\n  no certification names in it, so NO certifications could be read anonymously.\n  certifications is therefore an empty list meaning \"checked, nothing machine-readable\n  to record\" — not \"none held\". Because no named certification could\
  \ be verified, this\n  file deliberately does NOT emit a Compliance pointer.\nevidence:\n  - {source: 'https://trust.lytics.com/', http_status: 200, final_url: 'https://trust.contentstack.com/', bytes: 12718, rendered: client-side}\n  - {source: 'https://docs.lytics.com/docs/consent.md', http_status: 200, kind: docs-reference-to-trust-center}\n  - {source: 'https://www.lytics.com/security', http_status: 404}\n  - {source: 'https://www.lytics.com/.well-known/security.txt', http_status: 404}\nprivacy_and_compliance_surface:\n  - {name: Privacy Policy, url: 'https://www.lytics.com/privacy-policy/', http_status: 200}\n  - {name: Terms of Service, url: 'https://www.lytics.com/terms-of-service/', http_status: 200}\n  - {name: Compliance (GDPR/CCPA data subject requests), url: 'https://docs.lytics.com/docs/compliance', http_status: 200}\n  - {name: Consent & Privacy guide, url: 'https://docs.lytics.com/docs/consent', http_status: 200}\n  - {name: Account security settings reference, url: 'https://docs.lytics.com/docs/security',\
  \ http_status: 200}\nvulnerability_disclosure:\n  found: false\n  note: >-\n    No security.txt on any host, no /security or /responsible-disclosure page on\n    lytics.com, and no bug-bounty program (HackerOne/Bugcrowd/Intigriti) found for\n    Lytics. probe-security-programs.py returned vdp=none. No Security or\n    VulnerabilityDisclosure pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/security/lytics-trust-center.yml
summary_line: trust center published
tags:
- Customer Data Platform
- CDP
- Personalization
- Segmentation
- User Profiles
- Behavioral Analytics
- Content Affinity
- Real-Time Data
- Marketing Automation
- Audience Activation
trust_url: https://trust.lytics.com/
---
