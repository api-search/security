---
api_specs:
- filename: imagekit-media-api-openapi.yml
  format: yaml
  label: ImageKit Media API
  slug: apis-json-v1-9-imagekit-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imagekit/refs/heads/main/openapi/imagekit-media-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: imagekit.io
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: imagekit.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: api.imagekit.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imagekit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImageKit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ImageKit
provider_slug: apis-json-v1-9-imagekit
slug: imagekit-domain-security
source_filename: imagekit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imagekit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.imagekit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: imagekit.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/security/imagekit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Images
- Video
- CDN
- Media
- Optimization
- Transformations
- Digital Asset Management
- DAM
- Storage
- Cache
- Upload
---
