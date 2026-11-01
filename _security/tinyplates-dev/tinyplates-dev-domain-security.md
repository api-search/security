---
api_specs:
- filename: tinyplates-dev-health-api-openapi.yml
  format: yaml
  label: tinyplates-dev Health API
  slug: tinyplates-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-health-api-openapi.yml
- filename: tinyplates-dev-ingredients-api-openapi.yml
  format: yaml
  label: tinyplates-dev Ingredients API
  slug: tinyplates-dev-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-ingredients-api-openapi.yml
- filename: tinyplates-dev-pantry-api-openapi.yml
  format: yaml
  label: tinyplates-dev Pantry API
  slug: tinyplates-dev-pantry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-pantry-api-openapi.yml
- filename: tinyplates-dev-popular-api-openapi.yml
  format: yaml
  label: tinyplates-dev Popular API
  slug: tinyplates-dev-popular-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-popular-api-openapi.yml
- filename: tinyplates-dev-recipes-api-openapi.yml
  format: yaml
  label: tinyplates-dev Recipes API
  slug: tinyplates-dev-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-recipes-api-openapi.yml
- filename: tinyplates-dev-root-api-openapi.yml
  format: yaml
  label: tinyplates-dev Root API
  slug: tinyplates-dev-root-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-root-api-openapi.yml
- filename: tinyplates-dev-search-api-openapi.yml
  format: yaml
  label: tinyplates-dev Search API
  slug: tinyplates-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-search-api-openapi.yml
- filename: tinyplates-dev-shoppinglist-api-openapi.yml
  format: yaml
  label: tinyplates-dev Shopping List API
  slug: tinyplates-dev-shoppinglist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-shoppinglist-api-openapi.yml
- filename: tinyplates-dev-status-api-openapi.yml
  format: yaml
  label: tinyplates-dev Status API
  slug: tinyplates-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-status-api-openapi.yml
- filename: tinyplates-dev-substitutions-api-openapi.yml
  format: yaml
  label: tinyplates-dev Substitutions API
  slug: tinyplates-dev-substitutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-substitutions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: tinyplates.dev
  spf: false
hosts:
- cert_expires: Jan 15 11:34:22 2027 GMT
  host: tinyplates.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tinyplates Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tinyplates-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: tinyplates-dev
provider_slug: tinyplates-dev
slug: tinyplates-dev-domain-security
source_filename: tinyplates-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tinyplates.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 11:34:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tinyplates.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tinyplates-dev/security/tinyplates-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API
- Food
- Recipes
- Search
- Developer
---
