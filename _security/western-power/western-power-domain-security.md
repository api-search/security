---
api_specs:
- filename: western-power-content-api-openapi.yml
  format: yaml
  label: Western Power Content API
  slug: western-power-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-content-api-openapi.yml
- filename: western-power-metadata-api-openapi.yml
  format: yaml
  label: Western Power Metadata API
  slug: western-power-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-metadata-api-openapi.yml
- filename: western-power-outages-api-openapi.yml
  format: yaml
  label: Western Power Outages API
  slug: western-power-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-outages-api-openapi.yml
- filename: western-power-query-api-openapi.yml
  format: yaml
  label: Western Power Query API
  slug: western-power-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-query-api-openapi.yml
- filename: western-power-search-api-openapi.yml
  format: yaml
  label: Western Power Search API
  slug: western-power-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: westernpower.com.au
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.westernpower.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: services.westernpower.com.au
  https: false
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.mywpprojects.westernpower.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Western Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Western Power, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Western Power
provider_slug: western-power
slug: western-power-domain-security
source_filename: western-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westernpower.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.westernpower.com.au\n  https: false\n- host: www.mywpprojects.westernpower.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: westernpower.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/security/western-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Network Distribution
- Smart Metering
- Open Data
- GIS
- Outages
---
