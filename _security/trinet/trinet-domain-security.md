---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trinet.com
  spf: false
hosts:
- cert_expires: Sep 19 15:53:52 2026 GMT
  host: www.trinet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: developers.trinet.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trinet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TriNet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: TriNet
provider_slug: trinet
slug: trinet-domain-security
source_filename: trinet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trinet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.trinet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: trinet.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trinet/refs/heads/main/security/trinet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- PEO
- Professional Employer Organization
- Payroll
- Benefits
- HRIS
- HCM
- Workforce Management
- Time Off
- Compliance
- Mid-Market
- Small Business
- Co-Employment
- Fortune 1000
---
