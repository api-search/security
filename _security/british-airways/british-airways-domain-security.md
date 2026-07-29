---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: britishairways.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ba.com
  spf: true
hosts:
- cert_expires: Dec  1 08:56:04 2026 GMT
  host: www.britishairways.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:29:48 2026 GMT
  host: ndc.ba.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: British Airways Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for British Airways, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: British Airways
provider_slug: british-airways
slug: british-airways-domain-security
source_filename: british-airways-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.britishairways.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:56:04 2026 GMT\n  hsts: null\n- host: ndc.ba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: britishairways.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-airways/refs/heads/main/security/british-airways-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Distribution
- NDC
- Booking
- Corporate Travel
- Airports
---
