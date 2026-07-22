---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ro.co
  spf: true
hosts:
- cert_expires: Oct 17 07:30:13 2026 GMT
  host: ro.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ro
provider_slug: ro
slug: ro-domain-security
source_filename: ro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ro.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 07:30:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ro.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ro/refs/heads/main/security/ro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telehealth
- Healthcare
- Digital Health
- Pharmacy
- Direct to Consumer
- Weight Management
- Fertility
---
