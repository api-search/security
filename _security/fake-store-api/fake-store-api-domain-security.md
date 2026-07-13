---
api_specs:
- filename: fake-store-api-openapi.yml
  format: yaml
  label: Fake Store API
  slug: fake-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fake-store-api/refs/heads/main/openapi/fake-store-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fakestoreapi.com
  spf: true
hosts:
- cert_expires: Sep 13 07:59:55 2026 GMT
  host: fakestoreapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fake Store Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fake Store API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fake Store API
provider_slug: fake-store-api
slug: fake-store-api-domain-security
source_filename: fake-store-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fakestoreapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:59:55 2026 GMT\n  hsts: null\ndomains:\n- domain: fakestoreapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fake-store-api/refs/heads/main/security/fake-store-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Customers
- Fake Data
- Orders
- Products
- Synthetic Data
---
