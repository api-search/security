---
api_specs:
- filename: tvmaze-public-openapi.yml
  format: yaml
  label: TVmaze Public API
  slug: tvmaze-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-public-openapi.yml
- filename: tvmaze-premium-openapi.yml
  format: yaml
  label: TVmaze Premium User API
  slug: tvmaze-premium-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-premium-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tvmaze.com
  spf: true
hosts:
- cert_expires: Sep  8 15:28:36 2026 GMT
  host: www.tvmaze.com
  hsts: true
  hsts_max_age: 2629800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 15:28:36 2026 GMT
  host: api.tvmaze.com
  hsts: true
  hsts_max_age: 2629800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 19:13:19 2026 GMT
  host: static.tvmaze.com
  hsts: true
  hsts_max_age: 2629800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvmaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TVmaze, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TVmaze
provider_slug: tvmaze
slug: tvmaze-domain-security
source_filename: tvmaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tvmaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 2629800\n- host: api.tvmaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 2629800\n- host: static.tvmaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2629800\ndomains:\n- domain: tvmaze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/security/tvmaze-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Video
- Television
- Streaming
- Schedule
- Metadata
- Entertainment
- Public APIs
---
