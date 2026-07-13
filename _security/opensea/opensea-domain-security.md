---
api_specs:
- filename: opensea-api.json
  format: json
  label: OpenSea NFT API
  slug: nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Collection API
  slug: collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Listing API
  slug: listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Offer API
  slug: offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Order API
  slug: order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Drops API
  slug: drops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: opensea.io
  spf: true
hosts:
- cert_expires: Aug 16 13:22:37 2026 GMT
  host: docs.opensea.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:42:10 2026 GMT
  host: api.opensea.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:42:10 2026 GMT
  host: stream-api.opensea.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OpenSea
provider_slug: opensea
slug: opensea-domain-security
source_filename: opensea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.opensea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:22:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opensea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:42:10 2026 GMT\n  hsts: null\n- host: stream-api.opensea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:42:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: opensea.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/security/opensea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Marketplace
- Web3
- Blockchain
- Trading
- Digital Assets
---
