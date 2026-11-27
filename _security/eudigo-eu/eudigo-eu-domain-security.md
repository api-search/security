---
api_specs:
- filename: eudigo-eu-deadlines-api-openapi.yml
  format: yaml
  label: Eudigo Deadlines API
  slug: eudigo-eu-deadlines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudigo-eu/openapi/eudigo-eu-deadlines-api-openapi.yml
- filename: eudigo-eu-developers-api-openapi.yml
  format: yaml
  label: Eudigo Developers API
  slug: eudigo-eu-developers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudigo-eu/openapi/eudigo-eu-developers-api-openapi.yml
- filename: eudigo-eu-index-api-openapi.yml
  format: yaml
  label: Eudigo Index API
  slug: eudigo-eu-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudigo-eu/openapi/eudigo-eu-index-api-openapi.yml
- filename: eudigo-eu-knowledge-api-openapi.yml
  format: yaml
  label: Eudigo Knowledge API
  slug: eudigo-eu-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudigo-eu/openapi/eudigo-eu-knowledge-api-openapi.yml
- filename: eudigo-eu-registers-api-openapi.yml
  format: yaml
  label: Eudigo Registers API
  slug: eudigo-eu-registers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudigo-eu/openapi/eudigo-eu-registers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eudigo.eu
  spf: true
hosts:
- cert_expires: Jan 10 11:25:56 2027 GMT
  host: eudigo.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eudigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eudigo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eudigo
provider_slug: eudigo-eu
slug: eudigo-eu-domain-security
source_filename: eudigo-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eudigo.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:25:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eudigo.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eudigo-eu/security/eudigo-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Identity
- EUDI Wallet
- EU
- Open Data
- Guides
---
