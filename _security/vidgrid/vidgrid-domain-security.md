---
api_specs:
- filename: vidgrid-openapi-original.json
  format: json
  label: VidGrid Content Management API
  slug: vidgrid-content-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-openapi-original.json
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
