---
api_specs:
- filename: tristero-assets-api-openapi.yml
  format: yaml
  label: Tristero Assets API
  slug: tristero-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-assets-api-openapi.yml
- filename: tristero-margin-api-openapi.yml
  format: yaml
  label: Tristero Margin API
  slug: tristero-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-margin-api-openapi.yml
- filename: tristero-orders-api-openapi.yml
  format: yaml
  label: Tristero Orders API
  slug: tristero-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-orders-api-openapi.yml
- filename: tristero-pricing-api-openapi.yml
  format: yaml
  label: Tristero Pricing API
  slug: tristero-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-pricing-api-openapi.yml
- filename: tristero-quotes-api-openapi.yml
  format: yaml
  label: Tristero Quotes API
  slug: tristero-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-quotes-api-openapi.yml
- filename: tristero-trading-api-openapi.yml
  format: yaml
  label: Tristero Trading API
  slug: tristero-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-trading-api-openapi.yml
- filename: tristero-wallets-api-openapi.yml
  format: yaml
  label: Tristero Wallets API
  slug: tristero-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tristero.com
  spf: true
hosts:
- cert_expires: Oct 18 01:00:03 2026 GMT
  host: tristero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 01:00:03 2026 GMT
  host: docs.tristero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 02:03:09 2026 GMT
  host: api.tristero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tristero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tristero, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tristero
provider_slug: tristero
slug: tristero-domain-security
source_filename: tristero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tristero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tristero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:00:03 2026 GMT\n  hsts: false\n- host: api.tristero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:03:09 2026 GMT\n  hsts: null\ndomains:\n- domain: tristero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/security/tristero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Trading
- DeFi
- Cross-Chain
- Web3
- Margin Trading
- Dark Pools
---
