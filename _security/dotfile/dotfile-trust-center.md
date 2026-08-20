---
api_specs:
- filename: dotfile-cases-openapi.yml
  format: yaml
  label: Dotfile API
  slug: dotfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotfile/refs/heads/main/openapi/dotfile-cases-openapi.yml
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Dotfile Trust Center
name_suffix: Trust Center
overview: Dotfile maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Dotfile
provider_slug: dotfile
slug: dotfile-trust-center
source_filename: dotfile-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://trust.dotfile.com/\nurl: https://trust.dotfile.com/\nprovider: Vanta Trust Center\ncertifications:\n- SOC 2\n- GDPR\nclaims:\n- claim: SOC 2 Certified\n  source: https://www.dotfile.com/\n- claim: GDPR Compliant\n  source: https://www.dotfile.com/\n- claim: EU-located servers\n  source: https://www.dotfile.com/\n- claim: 99.99% availability\n  source: https://www.dotfile.com/\n- claim: SSO / OIDC, audit log, advanced permissions, custom data retention policies\n  source: https://www.dotfile.com/\nevidence:\n- source: https://trust.dotfile.com/\n  http_status: 200\n  kind: trust-center\n  note: >-\n    Live Vanta-hosted trust center. Page <title> is \"Dotfile Trust Center\"; the shell is served by\n    assets.vanta.com. The certification list itself is rendered client-side, so the named certifications\n    below were read from Dotfile's own homepage security section rather than scraped from the trust center\
  \ DOM.\n- source: https://www.dotfile.com/\n  http_status: 200\n  kind: website-security-section\n  keywords:\n  - soc 2 certified\n  - gdpr compliant\n  - eu-located servers\n  - 99.99% availability\n  - sso/oidc\nnotes:\n- No published vulnerability-disclosure or bug-bounty program was found. /.well-known/security.txt returns\n  404 on www.dotfile.com and docs.dotfile.com; api.dotfile.com answers 401 on every path including\n  /.well-known/*. No /security, /responsible-disclosure or HackerOne/Bugcrowd/Intigriti page was located.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotfile/refs/heads/main/security/dotfile-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- KYB
- KYC
- AML
- Business Verification
- Identity Verification
- Compliance
- RegTech
- Onboarding
- Sanctions Screening
- Document Verification
- Fraud Detection
- Company Data
- Beneficial Ownership
- Case Management
- Electronic Signature
- Webhook
trust_url: https://trust.dotfile.com/
---
