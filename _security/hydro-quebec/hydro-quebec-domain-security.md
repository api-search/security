---
api_specs:
- filename: hydro-quebec-catalog-api-openapi.yml
  format: yaml
  label: Hydro-Québec Catalog API
  slug: hydro-quebec-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-catalog-api-openapi.yml
- filename: hydro-quebec-dataset-api-openapi.yml
  format: yaml
  label: Hydro-Québec Dataset API
  slug: hydro-quebec-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-dataset-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hydroquebec.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.hydroquebec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 16:41:03 2026 GMT
  host: donnees.hydroquebec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hydro Quebec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydro-Québec, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hydro-Québec
provider_slug: hydro-quebec
slug: hydro-quebec-domain-security
source_filename: hydro-quebec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hydroquebec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: donnees.hydroquebec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 16:41:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hydroquebec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/security/hydro-quebec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Energy Markets
- Renewables
- Open Data
- Demand Response
- Carbon
---
