---
api_specs:
- filename: yepapi-openapi-generated.yml
  format: yaml
  label: YepAPI API
  slug: yepapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yepapi/refs/heads/main/openapi/_ae-authored/yepapi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yepapi.com
  spf: true
hosts:
- cert_expires: Dec 24 15:48:19 2026 GMT
  host: www.yepapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yepapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YepAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: YepAPI
provider_slug: yepapi
slug: yepapi-domain-security
source_filename: yepapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yepapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 15:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: yepapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yepapi/refs/heads/main/security/yepapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SEO
- SERP
- WebScraping
- AIModels
- Marketing
---
