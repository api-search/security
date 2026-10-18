---
api_specs:
- filename: cex-io-accounts-api-openapi.yml
  format: yaml
  label: CEX.IO Accounts API
  slug: cex-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-accounts-api-openapi.yml
- filename: cex-io-fees-api-openapi.yml
  format: yaml
  label: CEX.IO Fees API
  slug: cex-io-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-fees-api-openapi.yml
- filename: cex-io-funding-api-openapi.yml
  format: yaml
  label: CEX.IO Funding API
  slug: cex-io-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-funding-api-openapi.yml
- filename: cex-io-history-api-openapi.yml
  format: yaml
  label: CEX.IO History API
  slug: cex-io-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-history-api-openapi.yml
- filename: cex-io-market-data-api-openapi.yml
  format: yaml
  label: CEX.IO Market Data API
  slug: cex-io-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-market-data-api-openapi.yml
- filename: cex-io-orders-api-openapi.yml
  format: yaml
  label: CEX.IO Orders API
  slug: cex-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-orders-api-openapi.yml
- filename: cex-io-private-api-openapi.yml
  format: yaml
  label: CEX.IO Private API
  slug: cex-io-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-private-api-openapi.yml
- filename: cex-io-public-api-openapi.yml
  format: yaml
  label: CEX.IO Public API
  slug: cex-io-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-public-api-openapi.yml
- filename: cex-io-public-market-data-api-openapi.yml
  format: yaml
  label: CEX.IO Public Market Data API
  slug: cex-io-public-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-public-market-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cex.io
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: cex.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cex Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CEX.IO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CEX.IO
provider_slug: cex-io
slug: cex-io-domain-security
source_filename: cex-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cex.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/security/cex-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- WebSocket
- Financial Services
---
