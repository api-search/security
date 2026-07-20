---
api_specs:
- filename: angelcam-openapi-original.yml
  format: yaml
  label: Angelcam API
  slug: angelcam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/angelcam/refs/heads/main/openapi/angelcam-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: angelcam.com
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: angelcam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Angelcam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AngelCam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AngelCam
provider_slug: angelcam
slug: angelcam-domain-security
source_filename: angelcam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: angelcam.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: angelcam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angelcam/refs/heads/main/security/angelcam-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Video Surveillance
- Cameras
- IP Camera
- Cloud Recording
- Video Streaming
- IoT
- ONVIF
- Security
- Webhooks
---
