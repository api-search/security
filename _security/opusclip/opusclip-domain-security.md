---
api_specs:
- filename: opusclip-openapi-original.json
  format: json
  label: OpusClip Clip API
  slug: opusclip-clip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opus.pro
  spf: true
hosts:
- cert_expires: Aug 22 18:01:23 2026 GMT
  host: api.opus.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opusclip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpusClip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpusClip
provider_slug: opusclip
slug: opusclip-domain-security
source_filename: opusclip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.opus.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:01:23 2026 GMT\n  hsts: false\ndomains:\n- domain: opus.pro\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/security/opusclip-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Video
- AI
- Video Editing
- Short-Form Video
- Social Media
- Content Creation
- MCP
- Developer API
---
