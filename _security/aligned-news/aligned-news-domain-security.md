---
api_specs:
- filename: aligned-news-openapi.yml
  format: yaml
  label: Aligned News
  slug: aligned-news
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-openapi.yml
- filename: aligned-news-openapi.yml
  format: yaml
  label: Aligned News REST API
  slug: aligned-news-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alignednews.com
  spf: true
hosts:
- cert_expires: Aug 11 23:33:41 2026 GMT
  host: alignednews.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aligned News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aligned News, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aligned News
provider_slug: aligned-news
slug: aligned-news-domain-security
source_filename: aligned-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alignednews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alignednews.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/security/aligned-news-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- News
- Intelligence
- MCP
- Signals
---
