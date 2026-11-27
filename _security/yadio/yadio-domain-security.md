---
api_specs:
- filename: yadio-conversion-api-openapi.yml
  format: yaml
  label: Yadio Conversion API
  slug: yadio-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yadio/openapi/yadio-conversion-api-openapi.yml
- filename: yadio-historical-api-openapi.yml
  format: yaml
  label: Yadio Historical API
  slug: yadio-historical-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yadio/openapi/yadio-historical-api-openapi.yml
- filename: yadio-market-api-openapi.yml
  format: yaml
  label: Yadio Market API
  slug: yadio-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yadio/openapi/yadio-market-api-openapi.yml
- filename: yadio-metadata-api-openapi.yml
  format: yaml
  label: Yadio Metadata API
  slug: yadio-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yadio/openapi/yadio-metadata-api-openapi.yml
- filename: yadio-rates-api-openapi.yml
  format: yaml
  label: Yadio Rates API
  slug: yadio-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yadio/openapi/yadio-rates-api-openapi.yml
- filename: yadio-utilities-api-openapi.yml
  format: yaml
  label: Yadio Utilities API
  slug: yadio-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yadio/openapi/yadio-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yadio.io
  spf: true
hosts:
- cert_expires: Jan 19 15:33:12 2027 GMT
  host: yadio.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yadio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yadio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yadio
provider_slug: yadio
slug: yadio-domain-security
source_filename: yadio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yadio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 15:33:12 2027 GMT\n  hsts: false\ndomains:\n- domain: yadio.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/yadio/security/yadio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
