---
api_specs:
- filename: crawleo-dev-crawl-api-openapi.yml
  format: yaml
  label: crawleo-dev Crawl API
  slug: crawleo-dev-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawleo-dev/openapi/crawleo-dev-crawl-api-openapi.yml
- filename: crawleo-dev-google-maps-api-openapi.yml
  format: yaml
  label: crawleo-dev Google Maps API
  slug: crawleo-dev-google-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawleo-dev/openapi/crawleo-dev-google-maps-api-openapi.yml
- filename: crawleo-dev-search-api-openapi.yml
  format: yaml
  label: crawleo-dev Search API
  slug: crawleo-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawleo-dev/openapi/crawleo-dev-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crawleo.dev
  spf: true
hosts:
- cert_expires: Dec 25 09:35:28 2026 GMT
  host: crawleo.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crawleo Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crawleo-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: crawleo-dev
provider_slug: crawleo-dev
slug: crawleo-dev-domain-security
source_filename: crawleo-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawleo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 09:35:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crawleo.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crawleo-dev/security/crawleo-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Search
- Crawling
- API
- MCP
---
