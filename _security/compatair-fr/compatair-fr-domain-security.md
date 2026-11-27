---
api_specs:
- filename: compatair-fr-changefeed-api-openapi.yml
  format: yaml
  label: CompatAir Changefeed API
  slug: compatair-fr-changefeed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatair-fr/openapi/compatair-fr-changefeed-api-openapi.yml
- filename: compatair-fr-compatibility-api-openapi.yml
  format: yaml
  label: CompatAir Compatibility API
  slug: compatair-fr-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatair-fr/openapi/compatair-fr-compatibility-api-openapi.yml
- filename: compatair-fr-evidence-api-openapi.yml
  format: yaml
  label: CompatAir Evidence API
  slug: compatair-fr-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatair-fr/openapi/compatair-fr-evidence-api-openapi.yml
- filename: compatair-fr-search-api-openapi.yml
  format: yaml
  label: CompatAir Search API
  slug: compatair-fr-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatair-fr/openapi/compatair-fr-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: compatair.fr
  spf: false
hosts:
- cert_expires: Jan  9 19:32:35 2027 GMT
  host: compatair.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CompatAir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompatAir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: CompatAir
provider_slug: compatair-fr
slug: compatair-fr-domain-security
source_filename: compatair-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compatair.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 19:32:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: compatair.fr\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/compatair-fr/security/compatair-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Air Compressors
- Pneumatic Tools
- Compatibility
- Product Data
- Industrial Equipment
- MCP
- France
---
