---
api_specs:
- filename: fcsapi-forex-api-openapi.yml
  format: yaml
  label: FCS API Forex API
  slug: fcsapi-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcsapi/refs/heads/main/openapi/fcsapi-forex-api-openapi.yml
- filename: fcsapi-raw-api-openapi.yml
  format: yaml
  label: FCS API Raw API
  slug: fcsapi-raw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcsapi/refs/heads/main/openapi/fcsapi-raw-api-openapi.yml
- filename: fcsapi-stock-api-openapi.yml
  format: yaml
  label: FCS API Stock API
  slug: fcsapi-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcsapi/refs/heads/main/openapi/fcsapi-stock-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fcsapi.com
  spf: true
hosts:
- cert_expires: Dec 31 06:08:51 2026 GMT
  host: fcsapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fcsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FCS API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FCS API
provider_slug: fcsapi
slug: fcsapi-domain-security
source_filename: fcsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fcsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:08:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fcsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fcsapi/refs/heads/main/security/fcsapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Foreign Exchange
- Cryptocurrency
- Stocks
- DataAPI
---
