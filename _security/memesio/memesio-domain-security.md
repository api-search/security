---
api_specs:
- filename: openapi
  format: yaml
  label: Memesio API
  slug: memesio-api
  spec_type: OpenAPI
  url: https://memesio.com/api/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memesio.com
  spf: true
hosts:
- cert_expires: Sep 15 03:49:02 2026 GMT
  host: memesio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memesio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memesio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Memesio
provider_slug: memesio
slug: memesio-domain-security
source_filename: memesio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memesio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:49:02 2026 GMT\n  hsts: false\ndomains:\n- domain: memesio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/security/memesio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Memes
- Media
- Image Generation
- Content
- Developer Tools
---
