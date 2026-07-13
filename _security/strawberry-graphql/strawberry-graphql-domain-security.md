---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: strawberry.rocks
  spf: true
hosts:
- cert_expires: Sep 14 06:23:30 2026 GMT
  host: strawberry.rocks
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:22:12 2026 GMT
  host: play.strawberry.rocks
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strawberry Graphql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strawberry GraphQL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Strawberry GraphQL
provider_slug: strawberry-graphql
slug: strawberry-graphql-domain-security
source_filename: strawberry-graphql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strawberry.rocks\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:23:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: play.strawberry.rocks\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:22:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: strawberry.rocks\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strawberry-graphql/refs/heads/main/security/strawberry-graphql-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- GraphQL
- Python
- Open Source
- Code First
- Federation
---
