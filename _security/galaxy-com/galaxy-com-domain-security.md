---
api_specs:
- filename: galaxy-com-ethereum-api-openapi.yml
  format: yaml
  label: Galaxy Ethereum API
  slug: galaxy-com-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galaxy-com/refs/heads/main/openapi/galaxy-com-ethereum-api-openapi.yml
- filename: galaxy-com-solana-api-openapi.yml
  format: yaml
  label: Galaxy Solana API
  slug: galaxy-com-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galaxy-com/refs/heads/main/openapi/galaxy-com-solana-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galaxy.com
  spf: true
hosts:
- cert_expires: Dec  7 13:12:50 2026 GMT
  host: www.galaxy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Galaxy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galaxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Galaxy
provider_slug: galaxy-com
slug: galaxy-com-domain-security
source_filename: galaxy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.galaxy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 13:12:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: galaxy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galaxy-com/refs/heads/main/security/galaxy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Staking
- Ethereum
- Solana
- Trading
- Custody
- Financial Services
---
