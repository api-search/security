---
api_specs:
- filename: openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: apis-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demo-openapi/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apis.io
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: developer.apis.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: search-api.apis.io
  https: false
kind: domain-security
layout: security
method: probed
name: Demo Openapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manage OpenAPI via GitHub Demo, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Manage OpenAPI via GitHub Demo
provider_slug: demo-openapi
slug: demo-openapi-domain-security
source_filename: demo-openapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\n- host: search-api.apis.io\n  https: false\ndomains:\n- domain: apis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demo-openapi/refs/heads/main/security/demo-openapi-domain-security.yml
summary_line: TLSv1.3
tags:
- APIs.json
- Demo
- GitHub
- OpenAPI
- Reference
- Search
---
