---
api_specs:
- filename: artlist-search-openapi-original.yml
  format: yaml
  label: Artlist Enterprise Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-search-openapi-original.yml
- filename: artlist-download-openapi-original.yml
  format: yaml
  label: Artlist Enterprise Download API
  slug: download
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-download-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artlist.io
  spf: true
hosts:
- cert_expires: Oct 13 13:18:51 2026 GMT
  host: artlist.io
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 09:34:26 2026 GMT
  host: developer.artlist.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 03:40:06 2026 GMT
  host: business.artlist.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artlist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artlist
provider_slug: artlist
slug: artlist-domain-security
source_filename: artlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artlist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:18:51 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: developer.artlist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 09:34:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: business.artlist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:40:06 2026 GMT\n  hsts: null\ndomains:\n- domain: artlist.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/security/artlist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Audio
- Media
- Stock Media
- Content Licensing
- Creative Tools
- Search
- Generative AI
- Video
---
