---
api_specs:
- filename: krakend-service-api-openapi.yml
  format: yaml
  label: KrakenD Service API
  slug: krakend-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/openapi/krakend-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: krakend.io
  spf: true
hosts:
- cert_expires: Sep 29 12:30:59 2026 GMT
  host: www.krakend.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Krakend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KrakenD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KrakenD
provider_slug: krakend
slug: krakend-domain-security
source_filename: krakend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.krakend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:30:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: krakend.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/security/krakend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aggregation
- API Gateway
- Go
- Open Source
---
