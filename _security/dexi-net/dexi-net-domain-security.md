---
api_specs:
- filename: dexi-net-bookmarks-api-openapi.yml
  format: yaml
  label: Dexi Bookmarks API
  slug: dexi-net-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dexi-net/openapi/dexi-net-bookmarks-api-openapi.yml
- filename: dexi-net-publisher-api-openapi.yml
  format: yaml
  label: Dexi Publisher API
  slug: dexi-net-publisher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dexi-net/openapi/dexi-net-publisher-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dexi.net
  spf: false
hosts:
- cert_expires: Dec 12 09:14:35 2026 GMT
  host: dexi.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dexi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dexi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Dexi
provider_slug: dexi-net
slug: dexi-net-domain-security
source_filename: dexi-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dexi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 09:14:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dexi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dexi-net/security/dexi-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Management
- Personal-Productivity
- Note Taking
- Bookmarking
- RSS-Feeds
---
