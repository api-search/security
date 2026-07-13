---
api_specs:
- filename: openapi.json
  format: json
  label: TheNewsAPI
  slug: thenewsapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenewsapi/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: thenewsapi.com
  spf: true
hosts:
- cert_expires: Aug 29 02:30:46 2026 GMT
  host: www.thenewsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 02:30:46 2026 GMT
  host: api.thenewsapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thenewsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheNewsAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: TheNewsAPI
provider_slug: thenewsapi
slug: thenewsapi-domain-security
source_filename: thenewsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thenewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:30:46 2026 GMT\n  hsts: false\n- host: api.thenewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:30:46 2026 GMT\n  hsts: null\ndomains:\n- domain: thenewsapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thenewsapi/refs/heads/main/security/thenewsapi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- news
- articles
- headlines
- media
- aggregation
- real-time
---
