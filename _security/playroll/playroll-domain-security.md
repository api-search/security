---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playroll.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: www.playroll.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: playroll.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playroll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playroll, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Playroll
provider_slug: playroll
slug: playroll-domain-security
source_filename: playroll-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.playroll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: playroll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: playroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playroll/refs/heads/main/security/playroll-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Employer of Record
- EOR
- Global Payroll
- Contractor Management
- Global Employment
- HRIS
- Compliance
---
