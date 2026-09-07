---
api_specs:
- filename: videoverse-magnifi-partner-openapi.yml
  format: yaml
  label: Magnifi Partner Integration API
  slug: magnifi-partner-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-magnifi-partner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vverse.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: videoverse.dev
  spf: true
hosts:
- cert_expires: Nov  8 15:41:49 2026 GMT
  host: vverse.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 06:12:45 2026 GMT
  host: docs.prod.videoverse.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Videoverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VideoVerse, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VideoVerse
provider_slug: videoverse
slug: videoverse-domain-security
source_filename: videoverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vverse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 15:41:49 2026 GMT\n  hsts: false\n- host: docs.prod.videoverse.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 06:12:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vverse.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: videoverse.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/security/videoverse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Artificial Intelligence
- Sports
- Media
- Broadcasting
- Video Editing
- Highlights
- Content Creation
- Machine Learning
- Webhooks
---
