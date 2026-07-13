---
api_specs:
- filename: uclapi.json
  format: json
  label: UCL API Room Bookings
  slug: roombookings
  spec_type: OpenAPI
  url: https://github.com/uclapi/uclapi-openapi/blob/master/uclapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucl.ac.uk
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: uclapi.com
  spf: false
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.ucl.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 15:20:09 2026 GMT
  host: uclapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: discovery.ucl.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UCL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UCL
provider_slug: ucl
slug: ucl-domain-security
source_filename: ucl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: uclapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:20:09 2026 GMT\n  hsts: false\n- host: discovery.ucl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ucl.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uclapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/security/ucl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Open Data
- Research
- Library
- Timetable
---
