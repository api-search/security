---
api_specs:
- filename: bubbles-openapi.yml
  format: yaml
  label: Bubble Data API
  slug: bubble-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bubbles/refs/heads/main/openapi/bubbles-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bubble.io
  spf: true
hosts:
- cert_expires: Aug 27 04:34:13 2026 GMT
  host: bubble.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 00:11:04 2026 GMT
  host: manual.bubble.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bubbles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bubble, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bubble
provider_slug: bubbles
slug: bubbles-domain-security
source_filename: bubbles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bubble.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 04:34:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: manual.bubble.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bubble.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bubbles/refs/heads/main/security/bubbles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Applications
- Low Code
- No Code
- Visual Programming
- Webhooks
- Web Apps
---
