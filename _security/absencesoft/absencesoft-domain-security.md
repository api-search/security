---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: absencesoft.com
  spf: true
hosts:
- cert_expires: Aug 19 16:23:50 2026 GMT
  host: absencesoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Absencesoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbsenceSoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AbsenceSoft
provider_slug: absencesoft
slug: absencesoft-domain-security
source_filename: absencesoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: absencesoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: absencesoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absencesoft/refs/heads/main/security/absencesoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Leave Management
- Absence Management
- Accommodations
- HR Tech
- Compliance
- FMLA
- ADA
- Human Resources
---
