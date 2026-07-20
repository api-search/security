---
api_specs:
- filename: d3-doma-openapi.json
  format: json
  label: Doma Protocol API
  slug: doma-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d3/refs/heads/main/openapi/d3-doma-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: d3.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: doma.xyz
  spf: true
hosts:
- cert_expires: Sep 25 06:41:24 2026 GMT
  host: d3.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 01:23:51 2026 GMT
  host: docs.doma.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:06:07 2026 GMT
  host: api.doma.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D3, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: D3
provider_slug: d3
slug: d3-domain-security
source_filename: d3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: d3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:41:24 2026 GMT\n  hsts: false\n- host: docs.doma.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.doma.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:06:07 2026 GMT\n  hsts: null\ndomains:\n- domain: d3.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: doma.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d3/refs/heads/main/security/d3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Infrastructure
- Domains
- DNS
- Blockchain
- Tokenization
- Web3
- DomainFi
- Marketplace
- Agentic Commerce
---
