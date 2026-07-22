---
api_specs:
- filename: wideo-automation-openapi.yml
  format: yaml
  label: Wideo Video Automation API
  slug: wideo-video-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/openapi/wideo-automation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wideo.co
  spf: true
hosts:
- cert_expires: Sep  1 03:56:48 2026 GMT
  host: wideo.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: automationapi.wideo.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wideo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wideo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wideo
provider_slug: wideo
slug: wideo-domain-security
source_filename: wideo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wideo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:56:48 2026 GMT\n  hsts: false\n- host: automationapi.wideo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wideo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/security/wideo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Video Automation
- Content Creation
- Media
- Marketing
- Templates
- No-Code
---
