---
api_specs:
- filename: pg-and-e-authorization-api-openapi.yml
  format: yaml
  label: pg-and-e Authorization API
  slug: pg-and-e-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-authorization-api-openapi.yml
- filename: pg-and-e-subscriptions-api-openapi.yml
  format: yaml
  label: pg-and-e Subscriptions API
  slug: pg-and-e-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-subscriptions-api-openapi.yml
- filename: pg-and-e-usage-api-openapi.yml
  format: yaml
  label: pg-and-e Usage API
  slug: pg-and-e-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pge.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.pge.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: api.pge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Pg And E Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pg And E, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pg And E
provider_slug: pg-and-e
slug: pg-and-e-domain-security
source_filename: pg-and-e-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2628000\n- host: api.pge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/security/pg-and-e-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Energy
- Utilities
- Electricity
- Natural Gas
- California
- United States
- Smart Metering
- Green Button
- ESPI
- Energy Usage Data
- Investor-Owned Utility
- Customer Data Access
---
