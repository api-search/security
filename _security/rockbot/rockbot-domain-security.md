---
api_specs:
- filename: rockbot-openapi.yml
  format: yaml
  label: Rockbot API
  slug: rockbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "comodoca.com"
  - 0 issue "pki.goog"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rockbot.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: rockbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: developer.rockbot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.rockbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rockbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockbot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rockbot
provider_slug: rockbot
slug: rockbot-domain-security
source_filename: rockbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rockbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.rockbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.rockbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rockbot.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"comodoca.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/security/rockbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Music
- Digital Signage
- Audio Messaging
- Retail Media
- In-Location Media
- Media
- Entertainment
---
