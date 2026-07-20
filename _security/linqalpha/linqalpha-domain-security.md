---
api_specs:
- filename: linqalpha-openapi-original.json
  format: json
  label: LinqAlpha API
  slug: linqalpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linqalpha/refs/heads/main/openapi/linqalpha-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linqalpha.com
  spf: true
hosts:
- cert_expires: Sep 13 02:32:12 2026 GMT
  host: linqalpha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.linqalpha.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linqalpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinqAlpha, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LinqAlpha
provider_slug: linqalpha
slug: linqalpha-domain-security
source_filename: linqalpha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linqalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:32:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.linqalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: linqalpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linqalpha/refs/heads/main/security/linqalpha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Investment Research
- Artificial Intelligence
- Agents
- Market Data
- Equities
- Economic Data
- SEC Filings
- Retrieval Augmented Generation
- MCP
---
