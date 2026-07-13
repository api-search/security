---
api_specs:
- filename: the-news-api-openapi.yml
  format: yaml
  label: The News API
  slug: the-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-news-api/refs/heads/main/openapi/the-news-api-openapi.yml
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
name: The News Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The News API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: The News API
provider_slug: the-news-api
slug: the-news-api-domain-security
source_filename: the-news-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thenewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:30:46 2026 GMT\n  hsts: false\n- host: api.thenewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:30:46 2026 GMT\n  hsts: null\ndomains:\n- domain: thenewsapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-news-api/refs/heads/main/security/the-news-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Articles
- Headlines
- News
- Media
- Search
- International
---
