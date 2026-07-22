---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: graphql.org
  spf: false
hosts:
- cert_expires: Sep  8 20:56:08 2026 GMT
  host: graphql.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraphQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GraphQL
provider_slug: graphql
slug: graphql-domain-security
source_filename: graphql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphql.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:56:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: graphql.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphql/refs/heads/main/security/graphql-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data Fetching
- GraphQL
- Query Language
- Specification
---
