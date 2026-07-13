---
api_specs:
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale File Upload API
  slug: bytescale-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale Files Management API
  slug: bytescale-files-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale Image / Video Processing API
  slug: bytescale-image-video-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale CDN / Serving API
  slug: bytescale-cdn-serving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bytescale.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.bytescale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.bytescale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bytescale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bytescale, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bytescale
provider_slug: bytescale
slug: bytescale-domain-security
source_filename: bytescale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bytescale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bytescale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bytescale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/security/bytescale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Upload
- Storage
- Image Processing
- CDN
- Media
---
