---
api_specs:
- filename: opus-openapi-original.json
  format: json
  label: OpusClip API
  slug: opusclip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opus.pro
  spf: true
hosts:
- cert_expires: Sep  8 15:03:12 2026 GMT
  host: www.opus.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 17:58:13 2026 GMT
  host: help.opus.pro
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 18:01:23 2026 GMT
  host: api.opus.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Opus
provider_slug: opus
slug: opus-domain-security
source_filename: opus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opus.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:03:12 2026 GMT\n  hsts: false\n- host: help.opus.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 17:58:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.opus.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:01:23 2026 GMT\n  hsts: false\ndomains:\n- domain: opus.pro\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/security/opus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Frontier Tech
- Video
- AI
- Video Editing
- Short-Form Video
- Content Creation
- Social Media
- Media
- Agents
---
