---
api_specs:
- filename: graphiql
  format: yaml
  label: SanAPI
  slug: sanapi
  spec_type: OpenAPI
  url: https://api.santiment.net/graphiql
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: santiment.net
  spf: true
hosts:
- cert_expires: Sep 18 20:39:17 2026 GMT
  host: academy.santiment.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:39:17 2026 GMT
  host: api.santiment.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:39:17 2026 GMT
  host: sheets.santiment.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Santiment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santiment, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Santiment
provider_slug: santiment
slug: santiment-domain-security
source_filename: santiment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: academy.santiment.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:39:17 2026 GMT\n  hsts: false\n- host: api.santiment.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:39:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sheets.santiment.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:39:17 2026 GMT\n  hsts: false\ndomains:\n- domain: santiment.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santiment/refs/heads/main/security/santiment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto
- Blockchain
- Market Intelligence
- On-Chain Metrics
- Social Sentiment
- Developer Activity
- Analytics
- GraphQL
---
