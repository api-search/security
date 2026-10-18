---
api_specs:
- filename: btse-account-api-openapi.yml
  format: yaml
  label: BTSE Account API
  slug: btse-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-account-api-openapi.yml
- filename: btse-earn-api-openapi.yml
  format: yaml
  label: BTSE Earn API
  slug: btse-earn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-earn-api-openapi.yml
- filename: btse-markets-api-openapi.yml
  format: yaml
  label: BTSE Markets API
  slug: btse-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-markets-api-openapi.yml
- filename: btse-otc-api-openapi.yml
  format: yaml
  label: BTSE OTC API
  slug: btse-otc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-otc-api-openapi.yml
- filename: btse-trade-api-openapi.yml
  format: yaml
  label: BTSE Trade API
  slug: btse-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-trade-api-openapi.yml
- filename: btse-trade-v3-api-openapi.yml
  format: yaml
  label: BTSE Trade V3 API
  slug: btse-trade-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-trade-v3-api-openapi.yml
- filename: btse-trade-v4-api-openapi.yml
  format: yaml
  label: BTSE Trade V4 API
  slug: btse-trade-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-trade-v4-api-openapi.yml
- filename: btse-wallet-api-openapi.yml
  format: yaml
  label: BTSE Wallet API
  slug: btse-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: btse.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.btse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Btse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BTSE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BTSE
provider_slug: btse
slug: btse-domain-security
source_filename: btse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.btse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: btse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/security/btse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Digital Assets
- Futures
- WebSocket
---
