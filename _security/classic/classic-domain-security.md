---
api_specs:
- filename: classic-affiliate-api-openapi.yml
  format: yaml
  label: Classic Affiliate API
  slug: classic-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/openapi/classic-affiliate-api-openapi.yml
- filename: classic-auth-api-openapi.yml
  format: yaml
  label: Classic Auth API
  slug: classic-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/openapi/classic-auth-api-openapi.yml
- filename: classic-supported-assets-api-openapi.yml
  format: yaml
  label: Classic Supported Assets API
  slug: classic-supported-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/openapi/classic-supported-assets-api-openapi.yml
- filename: classic-supported-chains-api-openapi.yml
  format: yaml
  label: Classic Supported Chains API
  slug: classic-supported-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/openapi/classic-supported-chains-api-openapi.yml
- filename: classic-swaps-api-openapi.yml
  format: yaml
  label: Classic Swaps API
  slug: classic-swaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/openapi/classic-swaps-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: shapeshift.com
  spf: true
hosts:
- cert_expires: Oct 14 17:34:04 2026 GMT
  host: classic.shapeshift.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Classic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Classic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Classic
provider_slug: classic
slug: classic-domain-security
source_filename: classic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classic.shapeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shapeshift.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/security/classic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- DEX Aggregator
- Swaps
- Blockchain
- Wallets
- Self-Custody
---
