---
api_specs:
- filename: blazephoenix-xyz-abi-api-openapi.yml
  format: yaml
  label: BlazePhoenix Abi API
  slug: blazephoenix-xyz-abi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-abi-api-openapi.yml
- filename: blazephoenix-xyz-badge-api-openapi.yml
  format: yaml
  label: BlazePhoenix Badge API
  slug: blazephoenix-xyz-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-badge-api-openapi.yml
- filename: blazephoenix-xyz-blazephoenix-integration-api-your-rpc-api-openapi.yml
  format: yaml
  label: BlazePhoenix BlazePhoenix Integration API (your RPC) API
  slug: blazephoenix-xyz-blazephoenix-integration-api-your-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-blazephoenix-integration-api-your-rpc-api-openapi.yml
- filename: blazephoenix-xyz-deployments-api-openapi.yml
  format: yaml
  label: BlazePhoenix Deployments API
  slug: blazephoenix-xyz-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-deployments-api-openapi.yml
- filename: blazephoenix-xyz-health-api-openapi.yml
  format: yaml
  label: BlazePhoenix Health API
  slug: blazephoenix-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-health-api-openapi.yml
- filename: blazephoenix-xyz-manifest-api-openapi.yml
  format: yaml
  label: BlazePhoenix Manifest API
  slug: blazephoenix-xyz-manifest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-manifest-api-openapi.yml
- filename: blazephoenix-xyz-quote-api-openapi.yml
  format: yaml
  label: BlazePhoenix Quote API
  slug: blazephoenix-xyz-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-quote-api-openapi.yml
- filename: blazephoenix-xyz-stats-api-openapi.yml
  format: yaml
  label: BlazePhoenix Stats API
  slug: blazephoenix-xyz-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-stats-api-openapi.yml
- filename: blazephoenix-xyz-verify-api-openapi.yml
  format: yaml
  label: BlazePhoenix Verify API
  slug: blazephoenix-xyz-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blazephoenix.xyz
  spf: true
hosts:
- cert_expires: Dec  5 00:28:36 2026 GMT
  host: blazephoenix.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blazephoenix Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlazePhoenix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlazePhoenix
provider_slug: blazephoenix-xyz
slug: blazephoenix-xyz-domain-security
source_filename: blazephoenix-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blazephoenix.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 00:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blazephoenix.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blazephoenix-xyz/security/blazephoenix-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DeFi
- Decentralized Exchange
- Aggregator
- Onchain
---
