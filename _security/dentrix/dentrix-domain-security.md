---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dentrix.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: henryscheinone.com
  spf: true
hosts:
- cert_expires: Sep 25 16:56:03 2026 GMT
  host: www.dentrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 05:59:03 2026 GMT
  host: www.henryscheinone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dentrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dentrix, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dentrix
provider_slug: dentrix
slug: dentrix-domain-security
source_filename: dentrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dentrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:56:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.henryscheinone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dentrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: henryscheinone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dentrix/refs/heads/main/security/dentrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dental
- Practice Management
- Healthcare
- Dentistry
- Patient Data
- EHR
- Partner API
- Henry Schein One
---
