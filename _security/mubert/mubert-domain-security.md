---
api_specs:
- filename: mubert-music-api-openapi.yml
  format: yaml
  label: Mubert AI Music API
  slug: mubert-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mubert/refs/heads/main/openapi/mubert-music-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mubert.com
  spf: true
hosts:
- cert_expires: Aug 19 02:42:41 2026 GMT
  host: mubert.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 02:42:41 2026 GMT
  host: music-api.mubert.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mubert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mubert, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mubert
provider_slug: mubert
slug: mubert-domain-security
source_filename: mubert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mubert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:42:41 2026 GMT\n  hsts: false\n- host: music-api.mubert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:42:41 2026 GMT\n  hsts: null\ndomains:\n- domain: mubert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mubert/refs/heads/main/security/mubert-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Music
- Generative
- Royalty-Free
- Streaming
- Text-to-Music
- Image-to-Music
- Stems
- B2B
---
