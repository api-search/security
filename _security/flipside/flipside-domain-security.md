---
api_specs:
- filename: flipside-openapi.yml
  format: yaml
  label: Query Execution (SQL)
  slug: query-execution-sql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
- filename: flipside-openapi.yml
  format: yaml
  label: Query Results
  slug: query-results
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
- filename: flipside-openapi.yml
  format: yaml
  label: Datasets
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flipsidecrypto.xyz
  spf: false
hosts:
- cert_expires: Sep 19 15:13:43 2026 GMT
  host: flipsidecrypto.xyz
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:13:43 2026 GMT
  host: docs.flipsidecrypto.xyz
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: api-v2.flipsidecrypto.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Flipside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipside Crypto, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Flipside Crypto
provider_slug: flipside
slug: flipside-domain-security
source_filename: flipside-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flipsidecrypto.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:13:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.flipsidecrypto.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:13:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api-v2.flipsidecrypto.xyz\n  https: false\ndomains:\n- domain: flipsidecrypto.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/security/flipside-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Blockchain
- Analytics
- SQL
- Web3
- Data
---
