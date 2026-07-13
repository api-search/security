---
api_specs:
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Video Assets API
  slug: gumlet-video-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Video Collections API
  slug: gumlet-video-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Live Streaming API
  slug: gumlet-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Image Optimization API
  slug: gumlet-image-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Analytics API
  slug: gumlet-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Uploads API
  slug: gumlet-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gumlet.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.gumlet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:52:57 2026 GMT
  host: docs.gumlet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.gumlet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gumlet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gumlet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gumlet
provider_slug: gumlet
slug: gumlet-domain-security
source_filename: gumlet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gumlet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.gumlet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:52:57 2026 GMT\n  hsts: null\n- host: api.gumlet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gumlet.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/security/gumlet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Streaming
- Image Optimization
- CDN
- Encoding
- Analytics
---
