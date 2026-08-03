---
api_specs:
- filename: brightseed-posts-api-openapi.yml
  format: yaml
  label: Brightseed posts API
  slug: brightseed-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-posts-api-openapi.yml
- filename: brightseed-pages-api-openapi.yml
  format: yaml
  label: Brightseed pages API
  slug: brightseed-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-pages-api-openapi.yml
- filename: brightseed-media-api-openapi.yml
  format: yaml
  label: Brightseed media API
  slug: brightseed-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-media-api-openapi.yml
- filename: brightseed-categories-api-openapi.yml
  format: yaml
  label: Brightseed categories API
  slug: brightseed-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-categories-api-openapi.yml
- filename: brightseed-tags-api-openapi.yml
  format: yaml
  label: Brightseed tags API
  slug: brightseed-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-tags-api-openapi.yml
- filename: brightseed-users-api-openapi.yml
  format: yaml
  label: Brightseed users API
  slug: brightseed-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-users-api-openapi.yml
- filename: brightseed-comments-api-openapi.yml
  format: yaml
  label: Brightseed comments API
  slug: brightseed-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-comments-api-openapi.yml
- filename: brightseed-search-api-openapi.yml
  format: yaml
  label: Brightseed search API
  slug: brightseed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-search-api-openapi.yml
- filename: brightseed-taxonomies-api-openapi.yml
  format: yaml
  label: Brightseed taxonomies API
  slug: brightseed-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-taxonomies-api-openapi.yml
- filename: brightseed-types-api-openapi.yml
  format: yaml
  label: Brightseed types API
  slug: brightseed-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-types-api-openapi.yml
- filename: brightseed-statuses-api-openapi.yml
  format: yaml
  label: Brightseed statuses API
  slug: brightseed-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/openapi/brightseed-statuses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightseedbio.com
  spf: true
hosts:
- cert_expires: Oct 20 16:36:53 2026 GMT
  host: www.brightseedbio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightseed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightseed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brightseed
provider_slug: brightseed
slug: brightseed-domain-security
source_filename: brightseed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightseedbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 16:36:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brightseedbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/security/brightseed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bioactives
- Artificial Intelligence
- Life Sciences
- Nutrition
- Ingredients
- Drug Discovery
- Agrifood
- Content API
- WordPress
---
