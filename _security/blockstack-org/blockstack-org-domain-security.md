---
api_specs:
- filename: blockstack-org-api-openapi-generated.yml
  format: yaml
  label: Stacks api API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockstack-org/openapi/_ae-authored/blockstack-org-api-openapi-generated.yml
- filename: blockstack-org-core-openapi-generated.yml
  format: yaml
  label: Stacks core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockstack-org/openapi/_ae-authored/blockstack-org-core-openapi-generated.yml
- filename: blockstack-org-stacks.js-openapi-generated.yml
  format: yaml
  label: Stacks stacks.js API
  slug: stacks.js-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockstack-org/openapi/_ae-authored/blockstack-org-stacks.js-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockstack.org
  spf: true
hosts:
- cert_expires: Dec  3 14:22:51 2026 GMT
  host: www.blockstack.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blockstack Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stacks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stacks
provider_slug: blockstack-org
slug: blockstack-org-domain-security
source_filename: blockstack-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blockstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 14:22:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockstack.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/blockstack-org/security/blockstack-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bitcoin Staking
- Self‑Custodial
- DeFi
- Smart Contracts
- Layer‑2
- Institutional Crypto
---
