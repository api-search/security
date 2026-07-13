---
api_specs:
- filename: cloudimage-openapi.yml
  format: yaml
  label: Cloudimage Image Transformation (URL API)
  slug: cloudimage-image-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
- filename: cloudimage-openapi.yml
  format: yaml
  label: Cloudimage Optimization & CDN API
  slug: cloudimage-optimization-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
- filename: cloudimage-openapi.yml
  format: yaml
  label: Cloudimage Video Transformation (URL API)
  slug: cloudimage-video-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
- filename: cloudimage-openapi.yml
  format: yaml
  label: Filerobot DAM Upload & Asset API
  slug: filerobot-dam-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudimage.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scaleflex.com
  spf: true
hosts:
- cert_expires: Oct  4 21:29:06 2026 GMT
  host: www.cloudimage.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 01:45:26 2026 GMT
  host: docs.cloudimage.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 16:09:44 2026 GMT
  host: developers.scaleflex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudimage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudimage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloudimage
provider_slug: cloudimage
slug: cloudimage-domain-security
source_filename: cloudimage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudimage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:29:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloudimage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 01:45:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.scaleflex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:09:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudimage.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: scaleflex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/security/cloudimage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Image Optimization
- Image CDN
- Resizing
- Transformation
- DAM
---
