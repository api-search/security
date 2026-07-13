---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nestjs.com
  spf: true
hosts:
- cert_expires: Aug 17 04:04:10 2026 GMT
  host: nestjs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nestjs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NestJS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NestJS
provider_slug: nestjs
slug: nestjs-domain-security
source_filename: nestjs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nestjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:04:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nestjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nestjs/refs/heads/main/security/nestjs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Frameworks
- GraphQL
- Microservices
- Node.js
- REST
- TypeScript
- WebSockets
---
