---
api_specs:
- filename: apiable-platform-api-openapi.json
  format: json
  label: Apiable Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-platform-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiable.io
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.apiable.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: developer.apiable.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apiable
provider_slug: apiable
slug: apiable-domain-security
source_filename: apiable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: developer.apiable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apiable.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/security/apiable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon API Gateway
- API Gateway
- API Monetization
- API Portal
- Developer Experience
- Developer Portal
- Kong
- Platform
- Self-Service
---
