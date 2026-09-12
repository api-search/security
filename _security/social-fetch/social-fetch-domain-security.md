---
api_specs:
- filename: openapi.json
  format: json
  label: Social Fetch REST API
  slug: social-fetch-rest-api
  spec_type: OpenAPI
  url: https://www.socialfetch.dev/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: socialfetch.dev
  spf: false
hosts:
- cert_expires: Nov  1 18:48:03 2026 GMT
  host: www.socialfetch.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 10:00:20 2026 GMT
  host: api.socialfetch.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Social Fetch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Social Fetch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Social Fetch
provider_slug: social-fetch
slug: social-fetch-domain-security
source_filename: social-fetch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.socialfetch.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 18:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.socialfetch.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 10:00:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: socialfetch.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/social-fetch/refs/heads/main/security/social-fetch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- social media
- web scraping
- data extraction
- social listening
- monitoring
- structured data
- JSON API
- REST
- MCP
- agent-native
- TypeScript SDK
- transcripts
- ads intelligence
---
