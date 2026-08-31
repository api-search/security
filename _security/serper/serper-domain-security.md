---
api_specs:
- filename: serper-autocomplete-api-openapi.yml
  format: yaml
  label: Serper Autocomplete API
  slug: serper-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-autocomplete-api-openapi.yml
- filename: serper-images-api-openapi.yml
  format: yaml
  label: Serper Images API
  slug: serper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-images-api-openapi.yml
- filename: serper-lens-api-openapi.yml
  format: yaml
  label: Serper Lens API
  slug: serper-lens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-lens-api-openapi.yml
- filename: serper-locations-api-openapi.yml
  format: yaml
  label: Serper Locations API
  slug: serper-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-locations-api-openapi.yml
- filename: serper-maps-api-openapi.yml
  format: yaml
  label: Serper Maps API
  slug: serper-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-maps-api-openapi.yml
- filename: serper-news-api-openapi.yml
  format: yaml
  label: Serper News API
  slug: serper-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-news-api-openapi.yml
- filename: serper-patents-api-openapi.yml
  format: yaml
  label: Serper Patents API
  slug: serper-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-patents-api-openapi.yml
- filename: serper-places-api-openapi.yml
  format: yaml
  label: Serper Places API
  slug: serper-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-places-api-openapi.yml
- filename: serper-reviews-api-openapi.yml
  format: yaml
  label: Serper Reviews API
  slug: serper-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-reviews-api-openapi.yml
- filename: serper-scholar-api-openapi.yml
  format: yaml
  label: Serper Scholar API
  slug: serper-scholar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-scholar-api-openapi.yml
- filename: serper-search-api-openapi.yml
  format: yaml
  label: Serper Search API
  slug: serper-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-search-api-openapi.yml
- filename: serper-shopping-api-openapi.yml
  format: yaml
  label: Serper Shopping API
  slug: serper-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-shopping-api-openapi.yml
- filename: serper-videos-api-openapi.yml
  format: yaml
  label: Serper Videos API
  slug: serper-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-videos-api-openapi.yml
- filename: serper-scrape-api-openapi.yml
  format: yaml
  label: Serper Scrape API
  slug: serper-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-scrape-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: serper.dev
  spf: true
hosts:
- cert_expires: Oct 28 16:36:14 2026 GMT
  host: serper.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 14:34:17 2026 GMT
  host: google.serper.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serper, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Serper
provider_slug: serper
slug: serper-domain-security
source_filename: serper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serper.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:36:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: google.serper.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:34:17 2026 GMT\n  hsts: null\ndomains:\n- domain: serper.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/security/serper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- SERP
- Google Search
- Artificial Intelligence
- LLM
- SEO
- Image
- News
- Maps
- Shopping
- Reviews
- Lens
- Scraping
- Locations
- SERP API
- Web Search
- Agents
- Patents
- Scholar
- Autocomplete
- Places
- Videos
---
