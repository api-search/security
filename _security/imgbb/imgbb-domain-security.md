---
api_specs:
- filename: imgbb-openapi.yml
  format: yaml
  label: ImgBB Image Upload API
  slug: image-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgbb/refs/heads/main/openapi/imgbb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imgbb.com
  spf: true
hosts:
- cert_expires: Sep 30 19:13:42 2026 GMT
  host: imgbb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 19:13:42 2026 GMT
  host: api.imgbb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imgbb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImgBB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ImgBB
provider_slug: imgbb
slug: imgbb-domain-security
source_filename: imgbb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imgbb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.imgbb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: imgbb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgbb/refs/heads/main/security/imgbb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Image Hosting
- Image Upload
- File Sharing
- Cloud Storage
- Media
- REST API
---
