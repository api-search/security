---
api_specs:
- filename: trongrid-accounts-api-openapi.yml
  format: yaml
  label: TronGrid Accounts API
  slug: trongrid-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trongrid/openapi/trongrid-accounts-api-openapi.yml
- filename: trongrid-assets-api-openapi.yml
  format: yaml
  label: TronGrid Assets API
  slug: trongrid-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trongrid/openapi/trongrid-assets-api-openapi.yml
- filename: trongrid-blocks-api-openapi.yml
  format: yaml
  label: TronGrid Blocks API
  slug: trongrid-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trongrid/openapi/trongrid-blocks-api-openapi.yml
- filename: trongrid-contracts-api-openapi.yml
  format: yaml
  label: TronGrid Contracts API
  slug: trongrid-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trongrid/openapi/trongrid-contracts-api-openapi.yml
- filename: trongrid-transactions-api-openapi.yml
  format: yaml
  label: TronGrid Transactions API
  slug: trongrid-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trongrid/openapi/trongrid-transactions-api-openapi.yml
- filename: trongrid-trc20-api-openapi.yml
  format: yaml
  label: TronGrid Trc20 API
  slug: trongrid-trc20-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trongrid/openapi/trongrid-trc20-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trongrid.io
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: trongrid.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TronGrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TronGrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TronGrid
provider_slug: trongrid
slug: trongrid-domain-security
source_filename: trongrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trongrid.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trongrid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/trongrid/security/trongrid-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Blockchain
- Developer Tools
- Decentralized Applications
- TRON
- BTTC
---
