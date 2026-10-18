---
api_specs:
- filename: suggix-indicators-api-openapi.yml
  format: yaml
  label: Suggix Indicators API
  slug: suggix-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-indicators-api-openapi.yml
- filename: suggix-industries-api-openapi.yml
  format: yaml
  label: Suggix Industries API
  slug: suggix-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-industries-api-openapi.yml
- filename: suggix-regions-api-openapi.yml
  format: yaml
  label: Suggix Regions API
  slug: suggix-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-regions-api-openapi.yml
- filename: suggix-search-api-openapi.yml
  format: yaml
  label: Suggix Search API
  slug: suggix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-search-api-openapi.yml
- filename: suggix-sources-api-openapi.yml
  format: yaml
  label: Suggix Sources API
  slug: suggix-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-sources-api-openapi.yml
- filename: suggix-statistics-api-openapi.yml
  format: yaml
  label: Suggix Statistics API
  slug: suggix-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-statistics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: suggix.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.suggix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Suggix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suggix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Suggix
provider_slug: suggix
slug: suggix-domain-security
source_filename: suggix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suggix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: suggix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/security/suggix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software-as-a-Service
- Feedback
- Roadmaps
- Changelog
- Product Management
---
