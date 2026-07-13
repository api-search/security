---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Qobuz Music API
  slug: music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qobuz/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qobuz.com
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: www.qobuz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qobuz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qobuz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qobuz
provider_slug: qobuz
slug: qobuz-domain-security
source_filename: qobuz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qobuz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: qobuz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qobuz/refs/heads/main/security/qobuz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music Streaming
- Hi-Res Audio
- FLAC
- Lossless Audio
- Music Downloads
- Catalog Search
- Streaming URLs
- Music Metadata
- Audiophile
- France
---
