---
api_specs:
- filename: felt-felt-rest-api-openapi.yml
  format: yaml
  label: Felt REST API
  slug: felt-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-felt-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: felt.com
  spf: true
hosts:
- cert_expires: Aug 21 03:57:37 2026 GMT
  host: felt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:35:33 2026 GMT
  host: developers.felt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Felt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Felt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Felt
provider_slug: felt
slug: felt-domain-security
source_filename: felt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: felt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:57:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.felt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: felt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/security/felt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maps
- GIS
- Geospatial
- Collaborative
- Mapping
- Layers
- Embedding
---
