---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: planetdds.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: denticon.com
  spf: true
hosts:
- cert_expires: Sep 14 18:01:43 2026 GMT
  host: www.planetdds.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developer.planetdds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.denticon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Denticon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Denticon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Denticon
provider_slug: denticon
slug: denticon-domain-security
source_filename: denticon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planetdds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.planetdds.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.denticon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: planetdds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: denticon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denticon/refs/heads/main/security/denticon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dental
- Practice Management
- Healthcare
- DSO
- EHR
- Patient Data
- Revenue Cycle Management
- Partner API
---
