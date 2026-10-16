---
api_specs:
- filename: hourtick-v1-openapi.json
  format: json
  label: Hourtick API V1 API
  slug: hourtick-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/_original/hourtick-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hourtick.com
  spf: true
hosts:
- cert_expires: Jan  5 06:16:30 2027 GMT
  host: hourtick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hourtick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hourtick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hourtick
provider_slug: hourtick
slug: hourtick-domain-security
source_filename: hourtick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hourtick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:16:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hourtick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/security/hourtick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Collaboration
- AI
- TimeTracking
- ProjectManagement
---
