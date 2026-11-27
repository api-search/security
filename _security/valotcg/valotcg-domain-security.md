---
api_specs:
- filename: valotcg-analysis-api-openapi.yml
  format: yaml
  label: Valo.Data Analysis API
  slug: valotcg-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-analysis-api-openapi.yml
- filename: valotcg-cards-api-openapi.yml
  format: yaml
  label: Valo.Data Cards API
  slug: valotcg-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-cards-api-openapi.yml
- filename: valotcg-editions-api-openapi.yml
  format: yaml
  label: Valo.Data Editions API
  slug: valotcg-editions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-editions-api-openapi.yml
- filename: valotcg-games-api-openapi.yml
  format: yaml
  label: Valo.Data Games API
  slug: valotcg-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-games-api-openapi.yml
- filename: valotcg-sealed-api-openapi.yml
  format: yaml
  label: Valo.Data Sealed API
  slug: valotcg-sealed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-sealed-api-openapi.yml
- filename: valotcg-usage-api-openapi.yml
  format: yaml
  label: Valo.Data Usage API
  slug: valotcg-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: valotcg.com
  spf: true
hosts:
- cert_expires: Jan 27 21:39:02 2027 GMT
  host: valotcg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Valo.Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valo.Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Valo.Data
provider_slug: valotcg
slug: valotcg-domain-security
source_filename: valotcg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valotcg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 21:39:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: valotcg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/valotcg/security/valotcg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trading Card Games
- Pricing Data
- Vision
---
