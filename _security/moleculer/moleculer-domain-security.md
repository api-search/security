---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moleculer.services
  spf: true
hosts:
- cert_expires: Aug 25 17:38:54 2026 GMT
  host: moleculer.services
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moleculer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moleculer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Moleculer
provider_slug: moleculer
slug: moleculer-domain-security
source_filename: moleculer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moleculer.services\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:38:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moleculer.services\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moleculer/refs/heads/main/security/moleculer-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fault Tolerance
- Frameworks
- JavaScript
- Load Balancing
- Microservices
- Node.js
- Service Discovery
---
