---
api_specs:
- filename: capy-inc-captcha-openapi.yml
  format: yaml
  label: Lemin Captcha Verification API
  slug: lemin-captcha-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy-inc/refs/heads/main/openapi/capy-inc-captcha-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: leminnow.com
  spf: true
hosts:
- cert_expires: Sep 19 23:03:12 2026 GMT
  host: leminnow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:03:12 2026 GMT
  host: help.leminnow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:03:12 2026 GMT
  host: api.leminnow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capy Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capy Inc., probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Capy Inc.
provider_slug: capy-inc
slug: capy-inc-domain-security
source_filename: capy-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leminnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.leminnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:03:12 2026 GMT\n  hsts: false\n- host: api.leminnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:03:12 2026 GMT\n  hsts: false\ndomains:\n- domain: leminnow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capy-inc/refs/heads/main/security/capy-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- CAPTCHA
- Bot Detection
- Bot Prevention
- Fraud Prevention
- Account Takeover
- Authentication
- Web Security
- Developer Tools
---
