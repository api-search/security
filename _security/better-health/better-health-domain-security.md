---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinbetter.com
  spf: true
hosts:
- cert_expires: Aug 31 00:40:32 2026 GMT
  host: joinbetter.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Better Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Better Health
provider_slug: better-health
slug: better-health-domain-security
source_filename: better-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinbetter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:40:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: joinbetter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-health/refs/heads/main/security/better-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Supplies
- Diabetes
- CGM
- Ostomy
- Urology
- Incontinence
- Wound Care
- Direct to Consumer
- E-Commerce
---
