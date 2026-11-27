---
api_specs:
- filename: globalgov-io-agencies-api-openapi.yml
  format: yaml
  label: GlobalGov Agencies API
  slug: globalgov-io-agencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-agencies-api-openapi.yml
- filename: globalgov-io-awards-api-openapi.yml
  format: yaml
  label: GlobalGov Awards API
  slug: globalgov-io-awards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-awards-api-openapi.yml
- filename: globalgov-io-meta-api-openapi.yml
  format: yaml
  label: GlobalGov Meta API
  slug: globalgov-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-meta-api-openapi.yml
- filename: globalgov-io-solicitations-api-openapi.yml
  format: yaml
  label: GlobalGov Solicitations API
  slug: globalgov-io-solicitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-solicitations-api-openapi.yml
- filename: globalgov-io-vendors-api-openapi.yml
  format: yaml
  label: GlobalGov Vendors API
  slug: globalgov-io-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: globalgov.io
  spf: true
hosts:
- cert_expires: Jan  9 19:50:34 2027 GMT
  host: globalgov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GlobalGov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GlobalGov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GlobalGov
provider_slug: globalgov-io
slug: globalgov-io-domain-security
source_filename: globalgov-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globalgov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 19:50:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: globalgov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/globalgov-io/security/globalgov-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Procurement
- B2B
- Intelligence
- Platform
---
