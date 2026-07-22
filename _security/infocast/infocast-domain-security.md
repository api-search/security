---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: infocastinc.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: infocastinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infocast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infocast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Infocast
provider_slug: infocast
slug: infocast-domain-security
source_filename: infocast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infocastinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infocastinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infocast/refs/heads/main/security/infocast-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Conferences
- Energy
- Events
- Industry Intelligence
- Infrastructure
---
