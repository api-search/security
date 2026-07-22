---
api_specs:
- filename: mirage-openapi-original.json
  format: json
  label: Mirage Video API
  slug: mirage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: captions.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mirage.app
  spf: true
hosts:
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
name: Mirage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirage, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mirage
provider_slug: mirage
slug: mirage-domain-security
source_filename: mirage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: captions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:35:07 2026 GMT\n  hsts: false\n- host: api.mirage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:44:58 2026 GMT\n  hsts: null\ndomains:\n- domain: captions.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mirage.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/security/mirage-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Captions
- Media
- Content Creation
- Text to Speech
- Machine Learning
---
