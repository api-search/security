---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: byteport.com
  spf: true
hosts:
- cert_expires: Oct  1 01:03:49 2026 GMT
  host: byteport.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:38:31 2026 GMT
  host: docs.byteport.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.byteport.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Byteport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byteport, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Byteport
provider_slug: byteport
slug: byteport-domain-security
source_filename: byteport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byteport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.byteport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:38:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.byteport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: byteport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byteport/refs/heads/main/security/byteport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- File Transfer
- Data Transfer
- Acceleration
- Cloud Storage
- Robotics
- Artificial Intelligence
- Satellite
- Infrastructure
- Y Combinator
---
