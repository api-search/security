---
api_specs:
- filename: apipark-api.yaml
  format: yaml
  label: APIPark API
  slug: apipark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/openapi/apipark-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apipark.com
  spf: true
hosts:
- cert_expires: Sep  6 04:02:41 2026 GMT
  host: apipark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.apipark.com
  https: false
kind: domain-security
layout: security
method: probed
name: Apipark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIPark, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APIPark
provider_slug: apipark
slug: apipark-domain-security
source_filename: apipark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apipark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apipark.com\n  https: false\ndomains:\n- domain: apipark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/security/apipark-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- LLM
- Open Source
---
