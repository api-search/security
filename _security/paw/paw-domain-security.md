---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: paw.cloud
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: paw.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Paw
provider_slug: paw
slug: paw-domain-security
source_filename: paw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paw.cloud\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paw.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paw/refs/heads/main/security/paw-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- API Testing
- Clients
- HTTP Client
- macOS
---
