---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fastify.dev
  spf: true
hosts:
- cert_expires: Sep 29 15:49:20 2026 GMT
  host: fastify.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fastify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fastify
provider_slug: fastify
slug: fastify-domain-security
source_filename: fastify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:49:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: fastify.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastify/refs/heads/main/security/fastify-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Frameworks
- High Performance
- JavaScript
- JSON Schema
- Node.js
- TypeScript
---
