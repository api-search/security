---
api_specs:
- filename: vidgrid-caption-api-openapi.yml
  format: yaml
  label: VidGrid Caption API
  slug: vidgrid-caption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-caption-api-openapi.yml
- filename: vidgrid-folder-api-openapi.yml
  format: yaml
  label: VidGrid Folder API
  slug: vidgrid-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-folder-api-openapi.yml
- filename: vidgrid-search-api-openapi.yml
  format: yaml
  label: VidGrid Search API
  slug: vidgrid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-search-api-openapi.yml
- filename: vidgrid-token-api-openapi.yml
  format: yaml
  label: VidGrid Token API
  slug: vidgrid-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-token-api-openapi.yml
- filename: vidgrid-user-api-openapi.yml
  format: yaml
  label: VidGrid User API
  slug: vidgrid-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-user-api-openapi.yml
- filename: vidgrid-video-api-openapi.yml
  format: yaml
  label: VidGrid Video API
  slug: vidgrid-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-video-api-openapi.yml
- filename: vidgrid-webhooks-api-openapi.yml
  format: yaml
  label: VidGrid Webhooks API
  slug: vidgrid-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vidgrid.com
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: vidgrid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:46:47 2026 GMT
  host: developer.vidgrid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.vidgrid.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vidgrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VidGrid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VidGrid
provider_slug: vidgrid
slug: vidgrid-domain-security
source_filename: vidgrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vidgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.vidgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:46:47 2026 GMT\n  hsts: false\n- host: api.vidgrid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vidgrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/security/vidgrid-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Video
- Screen Recording
- Captions
- Video Hosting
- Webhooks
- Training
- HR
---
