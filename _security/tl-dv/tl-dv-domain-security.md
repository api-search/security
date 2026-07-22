---
api_specs:
- filename: tl-dv-openapi.yml
  format: yaml
  label: tl;dv API
  slug: tldv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tldv.io
  spf: true
hosts:
- cert_expires: Sep 27 04:06:04 2026 GMT
  host: tldv.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 04:06:04 2026 GMT
  host: pasta.tldv.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tl Dv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tl;dv, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: tl;dv
provider_slug: tl-dv
slug: tl-dv-domain-security
source_filename: tl-dv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tldv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:06:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: pasta.tldv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:06:04 2026 GMT\n  hsts: null\ndomains:\n- domain: tldv.io\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/security/tl-dv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Meetings
- Transcription
- Notetaking
- Conversation Intelligence
- Productivity
- Video
- Webhooks
- API
---
