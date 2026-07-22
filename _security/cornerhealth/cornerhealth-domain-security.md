---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cornerhealth.com
  spf: true
hosts:
- cert_expires: Oct  6 22:47:58 2026 GMT
  host: www.cornerhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cornerhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corner Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Corner Health
provider_slug: cornerhealth
slug: cornerhealth-domain-security
source_filename: cornerhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cornerhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:47:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cornerhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornerhealth/refs/heads/main/security/cornerhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Telehealth
- Nurse Practitioners
- Arizona
- Washington
---
