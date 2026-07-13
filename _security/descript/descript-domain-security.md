---
api_specs:
- filename: descript-openapi.yml
  format: yaml
  label: Descript Platform API
  slug: descript-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descript/refs/heads/main/openapi/descript-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: descript.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: descriptapi.com
  spf: false
hosts:
- cert_expires: Sep 15 22:38:37 2026 GMT
  host: www.descript.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 04:34:36 2026 GMT
  host: docs.descriptapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:39:28 2026 GMT
  host: descriptapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Descript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Descript, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Descript
provider_slug: descript
slug: descript-domain-security
source_filename: descript-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.descript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.descriptapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:34:36 2026 GMT\n  hsts: false\n- host: descriptapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:39:28 2026 GMT\n  hsts: false\ndomains:\n- domain: descript.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: descriptapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descript/refs/heads/main/security/descript-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Audio Editing
- Captions
- Media
- Podcasting
- Transcription
- Video Editing
---
