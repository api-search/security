---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trinet.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenefits.com
  spf: true
hosts:
- cert_expires: Sep 19 15:53:52 2026 GMT
  host: www.trinet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:53:48 2026 GMT
  host: developers.zenefits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.zenefits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zenefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TriNet Zenefits, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TriNet Zenefits
provider_slug: zenefits
slug: zenefits-domain-security
source_filename: zenefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trinet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.zenefits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zenefits.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trinet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zenefits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenefits/refs/heads/main/security/zenefits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Resources
- HRIS
- Payroll
- Benefits Administration
- Onboarding
- Time Tracking
---
