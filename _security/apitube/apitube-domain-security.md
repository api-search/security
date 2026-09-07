---
api_specs:
- filename: apitube-news-api-openapi.yml
  format: yaml
  label: APITube News API
  slug: apitube-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-news-api-openapi.yml
- filename: apitube-account-api-openapi.yml
  format: yaml
  label: APITube Account API
  slug: apitube-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-account-api-openapi.yml
- filename: apitube-fact-check-api-openapi.yml
  format: yaml
  label: APITube Fact Check API
  slug: apitube-fact-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-fact-check-api-openapi.yml
- filename: apitube-reference-api-openapi.yml
  format: yaml
  label: APITube Reference API
  slug: apitube-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-reference-api-openapi.yml
- filename: apitube-suggest-api-openapi.yml
  format: yaml
  label: APITube Suggest API
  slug: apitube-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-suggest-api-openapi.yml
- filename: apitube-system-api-openapi.yml
  format: yaml
  label: APITube System API
  slug: apitube-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-system-api-openapi.yml
- filename: apitube-utilities-api-openapi.yml
  format: yaml
  label: APITube Utilities API
  slug: apitube-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apitube.io
  spf: true
hosts:
- cert_expires: Nov  8 09:01:08 2026 GMT
  host: apitube.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 09:01:08 2026 GMT
  host: docs.apitube.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 09:01:08 2026 GMT
  host: api.apitube.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Apitube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APITube, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APITube
provider_slug: apitube
slug: apitube-domain-security
source_filename: apitube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apitube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 09:01:08 2026 GMT\n  hsts: false\n- host: docs.apitube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 09:01:08 2026 GMT\n  hsts: false\n- host: api.apitube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 09:01:08 2026 GMT\n  hsts: null\ndomains:\n- domain: apitube.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/security/apitube-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Media Monitoring
- News API
- Fact Check
- Journalists
---
