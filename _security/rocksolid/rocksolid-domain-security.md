---
api_specs:
- filename: rocksolid-allocations-api-openapi.yml
  format: yaml
  label: RockSolid Allocations API
  slug: rocksolid-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocksolid/refs/heads/main/openapi/rocksolid-allocations-api-openapi.yml
- filename: rocksolid-performance-api-openapi.yml
  format: yaml
  label: RockSolid Performance API
  slug: rocksolid-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocksolid/refs/heads/main/openapi/rocksolid-performance-api-openapi.yml
- filename: rocksolid-vaults-api-openapi.yml
  format: yaml
  label: RockSolid Vaults API
  slug: rocksolid-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocksolid/refs/heads/main/openapi/rocksolid-vaults-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rocksolid.network
  spf: false
hosts:
- cert_expires: Sep 13 00:33:24 2026 GMT
  host: rocksolid.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:58:47 2026 GMT
  host: app-integration.rocksolid.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rocksolid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RockSolid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: RockSolid
provider_slug: rocksolid
slug: rocksolid-domain-security
source_filename: rocksolid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rocksolid.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app-integration.rocksolid.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:58:47 2026 GMT\n  hsts: false\ndomains:\n- domain: rocksolid.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocksolid/refs/heads/main/security/rocksolid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DeFi
- Decentralized Finance
- Liquid Vaults
- Yield
- Staking
- Web3
- Blockchain
---
