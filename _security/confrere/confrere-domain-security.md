---
api_specs:
- filename: confrere-video-openapi.yml
  format: yaml
  label: Confrere Video API
  slug: confrere-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confrere/refs/heads/main/openapi/confrere-video-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: confrere.com
  spf: true
hosts:
- cert_expires: Jan 13 14:07:08 2027 GMT
  host: confrere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confrere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confrere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Confrere
provider_slug: confrere
slug: confrere-domain-security
source_filename: confrere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: confrere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 14:07:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: confrere.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confrere/refs/heads/main/security/confrere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Video
- Video Conferencing
- Communications
- Healthcare
- Telehealth
- Embeddable
- WebRTC
---
