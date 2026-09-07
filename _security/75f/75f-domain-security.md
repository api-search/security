---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 75f.io
  spf: true
hosts:
- cert_expires: Nov  6 16:13:48 2026 GMT
  host: www.75f.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:42:27 2026 GMT
  host: support.75f.io
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.75f.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 75F Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 75F, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 75F
provider_slug: 75f
slug: 75f-domain-security
source_filename: 75f-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.75f.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 16:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.75f.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.75f.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 75f.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/75f/refs/heads/main/security/75f-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Building Automation
- Smart Buildings
- HVAC
- Internet of Things
- Energy Management
- Project Haystack
- Facilities Management
- Sensors
- Building Management System
---
