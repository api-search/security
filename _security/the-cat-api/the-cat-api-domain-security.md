---
api_specs:
- filename: the-cat-api-breeds-api-openapi.yml
  format: yaml
  label: The Cat API Breeds API
  slug: the-cat-api-breeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-breeds-api-openapi.yml
- filename: the-cat-api-categories-api-openapi.yml
  format: yaml
  label: The Cat API Categories API
  slug: the-cat-api-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-categories-api-openapi.yml
- filename: the-cat-api-favourites-api-openapi.yml
  format: yaml
  label: The Cat API Favourites API
  slug: the-cat-api-favourites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-favourites-api-openapi.yml
- filename: the-cat-api-images-api-openapi.yml
  format: yaml
  label: The Cat API Images API
  slug: the-cat-api-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-images-api-openapi.yml
- filename: the-cat-api-votes-api-openapi.yml
  format: yaml
  label: The Cat API Votes API
  slug: the-cat-api-votes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-votes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thecatapi.com
  spf: true
hosts:
- cert_expires: Oct  4 11:18:35 2026 GMT
  host: thecatapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 11:18:35 2026 GMT
  host: api.thecatapi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Cat Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Cat API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: The Cat API
provider_slug: the-cat-api
slug: the-cat-api-domain-security
source_filename: the-cat-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thecatapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:18:35 2026 GMT\n  hsts: false\n- host: api.thecatapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:18:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: thecatapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/security/the-cat-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Animals
- Cats
- Image
- Media
---
