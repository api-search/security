---
api_specs:
- filename: adionics-posts-api-openapi.yml
  format: yaml
  label: Adionics Posts API
  slug: adionics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-posts-api-openapi.yml
- filename: adionics-pages-api-openapi.yml
  format: yaml
  label: Adionics Pages API
  slug: adionics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-pages-api-openapi.yml
- filename: adionics-media-api-openapi.yml
  format: yaml
  label: Adionics Media API
  slug: adionics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-media-api-openapi.yml
- filename: adionics-taxonomy-api-openapi.yml
  format: yaml
  label: Adionics Taxonomy API
  slug: adionics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-taxonomy-api-openapi.yml
- filename: adionics-search-api-openapi.yml
  format: yaml
  label: Adionics Search API
  slug: adionics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-search-api-openapi.yml
- filename: adionics-discovery-api-openapi.yml
  format: yaml
  label: Adionics Discovery API
  slug: adionics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: adionics.com
  spf: true
hosts:
- cert_expires: Dec  6 02:24:28 2026 GMT
  host: www.adionics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adionics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adionics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Adionics
provider_slug: adionics
slug: adionics-domain-security
source_filename: adionics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adionics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 02:24:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adionics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/security/adionics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Cleantech
- Lithium
- Direct Lithium Extraction
- Mining
- Battery Materials
- Water Treatment
- Desalination
- Geothermal
- Industrial Process Technology
- Sustainability
- Content
---
