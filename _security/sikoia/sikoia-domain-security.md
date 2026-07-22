---
api_specs:
- filename: sikoia-openapi.yml
  format: yaml
  label: Sikoia API
  slug: sikoia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sikoia.com
  spf: true
hosts:
- cert_expires: Oct 14 06:27:03 2026 GMT
  host: sikoia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sikoia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sikoia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sikoia
provider_slug: sikoia
slug: sikoia-domain-security
source_filename: sikoia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sikoia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:27:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sikoia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/security/sikoia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Identity Verification
- KYC
- KYB
- Onboarding
- Open Banking
- Credit
- Affordability
- Fraud & AML
- Document Verification
- RegTech
---
