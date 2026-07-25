---
api_specs:
- filename: superrare-collections-api-openapi.yml
  format: yaml
  label: SuperRare Collections API
  slug: superrare-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/openapi/superrare-collections-api-openapi.yml
- filename: superrare-media-api-openapi.yml
  format: yaml
  label: SuperRare Media API
  slug: superrare-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/openapi/superrare-media-api-openapi.yml
- filename: superrare-merkle-roots-api-openapi.yml
  format: yaml
  label: SuperRare Merkle Roots API
  slug: superrare-merkle-roots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/openapi/superrare-merkle-roots-api-openapi.yml
- filename: superrare-nfts-api-openapi.yml
  format: yaml
  label: SuperRare NFTs API
  slug: superrare-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/openapi/superrare-nfts-api-openapi.yml
- filename: superrare-tokens-api-openapi.yml
  format: yaml
  label: SuperRare Tokens API
  slug: superrare-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/openapi/superrare-tokens-api-openapi.yml
- filename: superrare-users-api-openapi.yml
  format: yaml
  label: SuperRare Users API
  slug: superrare-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/openapi/superrare-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: superrare.com
  spf: true
hosts:
- host: developer.superrare.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Jul 12 15:28:22 2026 GMT
  host: superrare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 12 15:28:22 2026 GMT
  host: api.superrare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superrare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuperRare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SuperRare
provider_slug: superrare
slug: superrare-domain-security
source_filename: superrare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.superrare.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: superrare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 12 15:28:22 2026 GMT\n  hsts: false\n- host: api.superrare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 12 15:28:22 2026 GMT\n  hsts: false\ndomains:\n- domain: superrare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superrare/refs/heads/main/security/superrare-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- NFT
- Digital Art
- Marketplace
- Ethereum
- Blockchain
- Auctions
- Collectibles
---
