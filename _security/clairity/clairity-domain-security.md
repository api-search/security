---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: clairitytech.com
  spf: true
hosts:
- cert_expires: Sep 19 06:49:54 2026 GMT
  host: clairitytech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clairity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clairity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Clairity
provider_slug: clairity
slug: clairity-domain-security
source_filename: clairity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clairitytech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clairitytech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clairity/refs/heads/main/security/clairity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Climate
- Carbon Removal
- Direct Air Capture
- Climate Tech
- Sustainability
---
