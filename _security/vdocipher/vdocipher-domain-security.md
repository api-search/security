---
api_specs:
- filename: vdocipher-folders-api-openapi.yml
  format: yaml
  label: VdoCipher Folders API
  slug: vdocipher-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-folders-api-openapi.yml
- filename: vdocipher-meta-api-openapi.yml
  format: yaml
  label: VdoCipher Meta API
  slug: vdocipher-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-meta-api-openapi.yml
- filename: vdocipher-playback-api-openapi.yml
  format: yaml
  label: VdoCipher Playback API
  slug: vdocipher-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-playback-api-openapi.yml
- filename: vdocipher-tags-api-openapi.yml
  format: yaml
  label: VdoCipher Tags API
  slug: vdocipher-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-tags-api-openapi.yml
- filename: vdocipher-upload-api-openapi.yml
  format: yaml
  label: VdoCipher Upload API
  slug: vdocipher-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-upload-api-openapi.yml
- filename: vdocipher-videos-api-openapi.yml
  format: yaml
  label: VdoCipher Videos API
  slug: vdocipher-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vdocipher.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.vdocipher.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: dev.vdocipher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vdocipher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VdoCipher, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VdoCipher
provider_slug: vdocipher
slug: vdocipher-domain-security
source_filename: vdocipher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vdocipher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\n- host: dev.vdocipher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vdocipher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/security/vdocipher-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Secure Video Hosting
- DRM
- Streaming
- E-Learning
- OTT
- Watermarking
---
