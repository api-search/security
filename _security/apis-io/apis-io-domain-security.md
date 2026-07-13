---
api_specs:
- filename: apis-io-v1-openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apis.io
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: apis.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: search-api.apis.io
  https: false
kind: domain-security
layout: security
method: probed
name: Apis Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIs.io, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APIs.io
provider_slug: apis-io
slug: apis-io-domain-security
source_filename: apis-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\n- host: search-api.apis.io\n  https: false\ndomains:\n- domain: apis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/security/apis-io-domain-security.yml
summary_line: TLSv1.3
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
---
