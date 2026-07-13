---
api_specs:
- filename: world-news-api-openapi.yml
  format: yaml
  label: World News API
  slug: world-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/world-news-api/refs/heads/main/openapi/world-news-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: worldnewsapi.com
  spf: false
hosts:
- cert_expires: Aug 19 16:57:47 2026 GMT
  host: worldnewsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:18:54 2026 GMT
  host: api.worldnewsapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: World News Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World News API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: World News API
provider_slug: world-news-api
slug: world-news-api-domain-security
source_filename: world-news-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worldnewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:57:47 2026 GMT\n  hsts: false\n- host: api.worldnewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:18:54 2026 GMT\n  hsts: null\ndomains:\n- domain: worldnewsapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-news-api/refs/heads/main/security/world-news-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
