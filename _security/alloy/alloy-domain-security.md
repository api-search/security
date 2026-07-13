---
api_specs:
- filename: llms.txt
  format: yaml
  label: Alloy Identity API
  slug: alloy-identity-api
  spec_type: OpenAPI
  url: https://developer.alloy.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alloy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alloy.co
  spf: true
hosts:
- cert_expires: Aug 24 11:19:46 2026 GMT
  host: www.alloy.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 21:53:47 2026 GMT
  host: developer.alloy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: sandbox.alloy.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alloy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alloy
provider_slug: alloy
slug: alloy-domain-security
source_filename: alloy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:19:46 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.alloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.alloy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alloy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: alloy.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/security/alloy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity Verification
- KYC
- KYB
- Fraud Prevention
- Compliance
- Onboarding
- Transaction Monitoring
- Risk Decisioning
- AML
- Fintech
---
