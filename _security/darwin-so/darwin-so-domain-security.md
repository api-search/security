---
api_specs:
- filename: darwin-so-account-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Account API
  slug: darwin-so-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-account-api-openapi.yml
- filename: darwin-so-accounts-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Accounts API
  slug: darwin-so-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-accounts-api-openapi.yml
- filename: darwin-so-act-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Act API
  slug: darwin-so-act-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-act-api-openapi.yml
- filename: darwin-so-search-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Search API
  slug: darwin-so-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: darwin.so
  spf: true
hosts:
- cert_expires: Jan 21 07:12:13 2027 GMT
  host: darwin.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Darwin So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Darwin Technologies, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Darwin Technologies, Inc.
provider_slug: darwin-so
slug: darwin-so-domain-security
source_filename: darwin-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: darwin.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 07:12:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: darwin.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/darwin-so/security/darwin-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Platform
- Developer Tools
- Marketplace
- Productivity
---
