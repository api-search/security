---
api_specs:
- filename: captions-mirage-openapi-original.json
  format: json
  label: Mirage Video API
  slug: mirage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-mirage-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mirage.app
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: captions.ai
  spf: true
hosts:
- cert_expires: Sep 29 23:30:41 2026 GMT
  host: platform.mirage.app
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:35:07 2026 GMT
  host: captions.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:44:58 2026 GMT
  host: api.mirage.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Captions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Captions
provider_slug: captions
slug: captions-domain-security
source_filename: captions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.mirage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:30:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: captions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:35:07 2026 GMT\n  hsts: false\n- host: api.mirage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:44:58 2026 GMT\n  hsts: null\ndomains:\n- domain: mirage.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: captions.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/security/captions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Video
- Artificial Intelligence
- Video Editing
- Video Generation
- Captions
- Subtitles
- Text to Speech
- AI Avatars
- Content Creation
- Media
---
