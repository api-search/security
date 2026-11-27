---
api_specs:
- filename: woz-api-nl-account-api-openapi.yml
  format: yaml
  label: woz-api-nl Account API
  slug: woz-api-nl-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-account-api-openapi.yml
- filename: woz-api-nl-adressen-api-openapi.yml
  format: yaml
  label: woz-api-nl Adressen API
  slug: woz-api-nl-adressen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-adressen-api-openapi.yml
- filename: woz-api-nl-lijst-api-openapi.yml
  format: yaml
  label: woz-api-nl Lijst API
  slug: woz-api-nl-lijst-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-lijst-api-openapi.yml
- filename: woz-api-nl-proef-api-openapi.yml
  format: yaml
  label: woz-api-nl Proef API
  slug: woz-api-nl-proef-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-proef-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: woz-api.nl
  spf: true
hosts:
- cert_expires: Jan 13 06:02:55 2027 GMT
  host: woz-api.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: woz-api-nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for woz-api-nl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: woz-api-nl
provider_slug: woz-api-nl
slug: woz-api-nl-domain-security
source_filename: woz-api-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woz-api.nl\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 06:02:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: woz-api.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/woz-api-nl/security/woz-api-nl-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Netherlands
- Property Valuation
- WOZ
---
