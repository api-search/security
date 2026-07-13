---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genql.dev
  spf: false
hosts:
- cert_expires: Sep 27 14:40:06 2026 GMT
  host: genql.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genql, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Genql
provider_slug: genql
slug: genql-domain-security
source_filename: genql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genql.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:40:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: genql.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genql/refs/heads/main/security/genql-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- GraphQL
- TypeScript
- Code Generation
- SDK
- Developer Tools
---
