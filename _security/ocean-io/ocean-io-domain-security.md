---
api_specs:
- filename: ocean-io-autocomplete-api-openapi.yml
  format: yaml
  label: Ocean.io Autocomplete API
  slug: ocean-io-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-autocomplete-api-openapi.yml
- filename: ocean-io-enrich-api-openapi.yml
  format: yaml
  label: Ocean.io Enrich API
  slug: ocean-io-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-enrich-api-openapi.yml
- filename: ocean-io-lookup-api-openapi.yml
  format: yaml
  label: Ocean.io Lookup API
  slug: ocean-io-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-lookup-api-openapi.yml
- filename: ocean-io-ocean-io-api-documentation-api-openapi.yml
  format: yaml
  label: Ocean.io Ocean.io API Documentation API
  slug: ocean-io-ocean-io-api-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-ocean-io-api-documentation-api-openapi.yml
- filename: ocean-io-other-api-openapi.yml
  format: yaml
  label: Ocean.io Other API
  slug: ocean-io-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-other-api-openapi.yml
- filename: ocean-io-reveal-api-openapi.yml
  format: yaml
  label: Ocean.io Reveal API
  slug: ocean-io-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-reveal-api-openapi.yml
- filename: ocean-io-search-api-openapi.yml
  format: yaml
  label: Ocean.io Search API
  slug: ocean-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-search-api-openapi.yml
- filename: ocean-io-segmentation-api-openapi.yml
  format: yaml
  label: Ocean.io Segmentation API
  slug: ocean-io-segmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-segmentation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ocean.io
  spf: true
hosts:
- cert_expires: Oct 10 21:42:14 2026 GMT
  host: ocean.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 21:42:14 2026 GMT
  host: api.ocean.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocean Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocean.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ocean.io
provider_slug: ocean-io
slug: ocean-io-domain-security
source_filename: ocean-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocean.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:42:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ocean.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:42:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ocean.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/security/ocean-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Intelligence
- B2B
- Enrichment
- Lookalike
- Account Based Marketing
- Prospecting
- Company Data
- People Data
- Contact Data
- Segmentation
- Go-To-Market
- MCP
---
