---
api_specs:
- filename: recipe-api-discovery-api-openapi.yml
  format: yaml
  label: Recipe API Discovery API
  slug: recipe-api-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-discovery-api-openapi.yml
- filename: recipe-api-image-generation-api-openapi.yml
  format: yaml
  label: Recipe API Image Generation API
  slug: recipe-api-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-image-generation-api-openapi.yml
- filename: recipe-api-ingredients-api-openapi.yml
  format: yaml
  label: Recipe API Ingredients API
  slug: recipe-api-ingredients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-ingredients-api-openapi.yml
- filename: recipe-api-public-api-openapi.yml
  format: yaml
  label: Recipe API Public API
  slug: recipe-api-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-public-api-openapi.yml
- filename: recipe-api-recipes-api-openapi.yml
  format: yaml
  label: Recipe API Recipes API
  slug: recipe-api-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-recipes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: recipeapi.io
  spf: true
hosts:
- cert_expires: Sep  7 13:04:41 2026 GMT
  host: recipeapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Recipe Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recipe API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Recipe API
provider_slug: recipe-api
slug: recipe-api-domain-security
source_filename: recipe-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recipeapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:04:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: recipeapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/security/recipe-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Recipes
- Food
- Nutrition
- Ingredients
- Data
- Generative AI
- MCP
- Agents
---
