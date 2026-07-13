---
api_specs:
- filename: eu-open-data-portal-search-openapi.yml
  format: yaml
  label: EU Open Data Portal Search API
  slug: eu-open-data-portal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-search-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: data.europa.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eu Open Data Portal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EU Open Data Portal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: EU Open Data Portal
provider_slug: eu-open-data-portal
slug: eu-open-data-portal-domain-security
source_filename: eu-open-data-portal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/security/eu-open-data-portal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Open Data
- SPARQL
- EU
- Regulatory
- Linked Data
---
