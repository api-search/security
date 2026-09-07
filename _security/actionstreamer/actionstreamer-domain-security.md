---
api_specs:
- filename: actionstreamer-openapi-original.json
  format: json
  label: ActionStreamer Web API
  slug: actionstreamer-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionstreamer/refs/heads/main/openapi/_original/actionstreamer-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: actionstreamer.com
  spf: true
hosts:
- cert_expires: Nov  1 15:06:24 2026 GMT
  host: actionstreamer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 08:31:44 2026 GMT
  host: developer.actionstreamer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 00:17:31 2026 GMT
  host: api.actionstreamer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Actionstreamer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActionStreamer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ActionStreamer
provider_slug: actionstreamer
slug: actionstreamer-domain-security
source_filename: actionstreamer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actionstreamer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:06:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.actionstreamer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 08:31:44 2026 GMT\n  hsts: false\n- host: api.actionstreamer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 00:17:31 2026 GMT\n  hsts: null\ndomains:\n- domain: actionstreamer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actionstreamer/refs/heads/main/security/actionstreamer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Live Streaming
- Wearables
- Internet of Things
- Device Management
- Public Safety
- Industrial
- Computer Vision
- Media
---
