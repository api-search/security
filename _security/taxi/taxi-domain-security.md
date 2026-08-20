---
api_specs:
- filename: taxi-conversion-api-openapi.yml
  format: yaml
  label: Taxi - Describe How Your APIs and Data Relate Conversion API
  slug: taxi-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxi/refs/heads/main/openapi/taxi-conversion-api-openapi.yml
- filename: taxi-queries-api-openapi.yml
  format: yaml
  label: Taxi - Describe How Your APIs and Data Relate Queries API
  slug: taxi-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxi/refs/heads/main/openapi/taxi-queries-api-openapi.yml
- filename: taxi-schemas-api-openapi.yml
  format: yaml
  label: Taxi - Describe How Your APIs and Data Relate Schemas API
  slug: taxi-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxi/refs/heads/main/openapi/taxi-schemas-api-openapi.yml
- filename: taxi-services-api-openapi.yml
  format: yaml
  label: Taxi - Describe How Your APIs and Data Relate Services API
  slug: taxi-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxi/refs/heads/main/openapi/taxi-services-api-openapi.yml
- filename: taxi-types-api-openapi.yml
  format: yaml
  label: Taxi - Describe How Your APIs and Data Relate Types API
  slug: taxi-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxi/refs/heads/main/openapi/taxi-types-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: taxilang.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orbitalhq.com
  spf: false
hosts:
- cert_expires: Oct  7 08:13:48 2026 GMT
  host: taxilang.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.taxilang.org
  https: false
- cert_expires: Sep 30 02:53:48 2026 GMT
  host: orbitalhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taxi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taxi - Describe How Your APIs and Data Relate, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Taxi - Describe How Your APIs and Data Relate
provider_slug: taxi
slug: taxi-domain-security
source_filename: taxi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taxilang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.taxilang.org\n  https: false\n- host: orbitalhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taxilang.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: orbitalhq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxi/refs/heads/main/security/taxi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Description
- Data Integration
- Open-Source
- Query Language
- Schema
- Semantic
---
