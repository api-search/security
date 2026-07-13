---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Landbot Platform API
  slug: landbot-platform-api
  spec_type: OpenAPI
  url: https://api.landbot.io/
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: landbot.io
  spf: true
hosts:
- cert_expires: Sep 12 21:00:21 2026 GMT
  host: landbot.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 13:49:14 2026 GMT
  host: dev.landbot.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 21:00:21 2026 GMT
  host: api.landbot.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landbot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Landbot
provider_slug: landbot
slug: landbot-domain-security
source_filename: landbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landbot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:00:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.landbot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:49:14 2026 GMT\n  hsts: false\n- host: api.landbot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:00:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: landbot.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landbot/refs/heads/main/security/landbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- chatbot
- conversational AI
- no-code
- WhatsApp
- webhooks
- messaging
- automation
---
