---
api_specs:
- filename: lingopal-openapi-original.json
  format: json
  label: Lingopal API v2
  slug: lingopal-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingopal/refs/heads/main/openapi/lingopal-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lingopal.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lingopal-dev.com
  spf: false
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: lingopal.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: vod-api.lingopal-dev.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lingopal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lingopal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lingopal
provider_slug: lingopal
slug: lingopal-domain-security
source_filename: lingopal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lingopal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: vod-api.lingopal-dev.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lingopal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lingopal-dev.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingopal/refs/heads/main/security/lingopal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Frontier Tech
- Artificial Intelligence
- Translation
- Localization
- Speech
- Media
- Broadcasting
- Video
- Subtitles
- Voice Cloning
---
