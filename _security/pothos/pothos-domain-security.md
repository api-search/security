---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: pothos-graphql.dev
  spf: false
hosts:
- cert_expires: Aug 16 18:58:49 2026 GMT
  host: pothos-graphql.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pothos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pothos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Pothos
provider_slug: pothos
slug: pothos-domain-security
source_filename: pothos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pothos-graphql.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:58:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pothos-graphql.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pothos/refs/heads/main/security/pothos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- GraphQL
- TypeScript
- Schema Builder
- Code First
- Plugin System
---
