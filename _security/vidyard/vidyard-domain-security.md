---
api_specs:
- filename: create.html
  format: yaml
  label: Vidyard Dashboard API
  slug: vidyard-dashboard-api
  spec_type: OpenAPI
  url: https://developer.vidyard.com/apidoc/api_videos/create.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vidyard.com
  spf: true
hosts:
- cert_expires: Aug 17 21:47:04 2026 GMT
  host: www.vidyard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: developer.vidyard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: api.vidyard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vidyard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vidyard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vidyard
provider_slug: vidyard
slug: vidyard-domain-security
source_filename: vidyard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vidyard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:47:04 2026 GMT\n  hsts: false\n- host: developer.vidyard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.vidyard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vidyard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidyard/refs/heads/main/security/vidyard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Video Platform
- Video Analytics
- Video Sharing
- Sales Video
- CRM Integration
- Marketing
- AI Video
- Webhooks
---
