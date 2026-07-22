---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tokaidohealth.com
  spf: false
hosts:
- cert_expires: Sep 11 13:34:30 2026 GMT
  host: tokaidohealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tokaidohealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tokaido Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Tokaido Health
provider_slug: tokaidohealth
slug: tokaidohealth-domain-security
source_filename: tokaidohealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tokaidohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:34:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tokaidohealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tokaidohealth/refs/heads/main/security/tokaidohealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- Medication
- Employee Benefits
- Artificial Intelligence
---
