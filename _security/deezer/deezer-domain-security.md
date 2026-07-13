---
api_specs:
- filename: deezer-openapi.yml
  format: yaml
  label: Deezer API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deezer.com
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.deezer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: developers.deezer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.deezer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deezer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deezer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deezer
provider_slug: deezer
slug: deezer-domain-security
source_filename: deezer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deezer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.deezer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.deezer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deezer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/security/deezer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Streaming
- Audio
- OAuth
- Catalog
- Playlists
---
