---
api_specs:
- filename: x2y2-chain-api-openapi.yml
  format: yaml
  label: X2Y2 Chain API
  slug: x2y2-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-chain-api-openapi.yml
- filename: x2y2-contracts-api-openapi.yml
  format: yaml
  label: X2Y2 Contracts API
  slug: x2y2-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-contracts-api-openapi.yml
- filename: x2y2-events-api-openapi.yml
  format: yaml
  label: X2Y2 Events API
  slug: x2y2-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-events-api-openapi.yml
- filename: x2y2-general-api-openapi.yml
  format: yaml
  label: X2Y2 General API
  slug: x2y2-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-general-api-openapi.yml
- filename: x2y2-loan-api-openapi.yml
  format: yaml
  label: X2Y2 Loan API
  slug: x2y2-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-loan-api-openapi.yml
- filename: x2y2-offer-api-openapi.yml
  format: yaml
  label: X2Y2 Offer API
  slug: x2y2-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-offer-api-openapi.yml
- filename: x2y2-offers-api-openapi.yml
  format: yaml
  label: X2Y2 Offers API
  slug: x2y2-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-offers-api-openapi.yml
- filename: x2y2-orders-api-openapi.yml
  format: yaml
  label: X2Y2 Orders API
  slug: x2y2-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/openapi/x2y2-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: x2y2.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: x2y2.org
  spf: true
hosts:
- cert_expires: Aug 24 07:47:08 2026 GMT
  host: docs.x2y2.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 21:28:39 2026 GMT
  host: api.x2y2.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 19:31:15 2026 GMT
  host: loan-api.x2y2.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: X2Y2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X2Y2, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: X2Y2
provider_slug: x2y2
slug: x2y2-domain-security
source_filename: x2y2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.x2y2.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:47:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.x2y2.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:28:39 2026 GMT\n  hsts: null\n- host: loan-api.x2y2.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:31:15 2026 GMT\n  hsts: false\ndomains:\n- domain: x2y2.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: x2y2.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/security/x2y2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Ethereum
- Marketplace
- Blockchain
- Web3
- Collectibles
- Trading
---
