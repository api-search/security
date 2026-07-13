---
api_specs:
- filename: imgur-openapi.yml
  format: yaml
  label: Imgur API v3
  slug: imgur-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgur/refs/heads/main/openapi/imgur-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imgur.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: imgur.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.imgur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 14 14:42:27 2026 GMT
  host: apidocs.imgur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imgur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imgur, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Imgur
provider_slug: imgur
slug: imgur-domain-security
source_filename: imgur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imgur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.imgur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.imgur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 14:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: imgur.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgur/refs/heads/main/security/imgur-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Photography
- Images
- Image Hosting
- Albums
- Gallery
- Social
- Memes
- Content Sharing
- Public APIs
---
