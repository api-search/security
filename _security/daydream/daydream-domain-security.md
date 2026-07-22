---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daydream.dental
  spf: true
hosts:
- cert_expires: Aug 23 04:14:05 2026 GMT
  host: daydream.dental
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daydream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DayDream Dental, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DayDream Dental
provider_slug: daydream
slug: daydream-domain-security
source_filename: daydream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daydream.dental\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 04:14:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: daydream.dental\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daydream/refs/heads/main/security/daydream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dental
- Billing
- Revenue Cycle Management
- Healthcare
- Insurance Verification
- Claims
- RCM
- Dental Service Organization
---
