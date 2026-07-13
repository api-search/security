---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: precisely.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: developer.precisely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 13 07:03:46 2026 GMT
  host: www.precisely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Precisely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Precisely, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Precisely
provider_slug: precisely
slug: precisely-domain-security
source_filename: precisely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.precisely.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.precisely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 07:03:46 2026 GMT\n  hsts: false\ndomains:\n- domain: precisely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precisely/refs/heads/main/security/precisely-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Address Verification
- Data Integrity
- Geocoding
- Location Intelligence
---
