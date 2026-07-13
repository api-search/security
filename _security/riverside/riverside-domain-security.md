---
api_specs:
- filename: riverside-business-openapi.yml
  format: yaml
  label: Riverside Business API
  slug: riverside-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/openapi/riverside-business-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: riverside.fm
  spf: true
hosts:
- cert_expires: Sep 25 12:34:05 2026 GMT
  host: riverside.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:05:06 2026 GMT
  host: docs.riverside.fm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:05:06 2026 GMT
  host: platform.riverside.fm
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riverside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riverside, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Riverside
provider_slug: riverside
slug: riverside-domain-security
source_filename: riverside-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: riverside.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:34:05 2026 GMT\n  hsts: false\n- host: docs.riverside.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:05:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.riverside.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:05:06 2026 GMT\n  hsts: null\ndomains:\n- domain: riverside.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/security/riverside-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcast
- Video Recording
- Media
- Content Creation
- Audio
---
