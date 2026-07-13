---
api_specs:
- filename: bot-butcher-openapi.yml
  format: yaml
  label: Bot Butcher Classification API
  slug: bot-butcher-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bot-butcher/refs/heads/main/openapi/bot-butcher-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: botbutcher.com
  spf: true
hosts:
- cert_expires: Sep 26 15:36:24 2026 GMT
  host: botbutcher.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 19:06:22 2026 GMT
  host: api.botbutcher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bot Butcher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bot Butcher, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bot Butcher
provider_slug: bot-butcher
slug: bot-butcher-domain-security
source_filename: bot-butcher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botbutcher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:36:24 2026 GMT\n  hsts: false\n- host: api.botbutcher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:06:22 2026 GMT\n  hsts: null\ndomains:\n- domain: botbutcher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bot-butcher/refs/heads/main/security/bot-butcher-domain-security.yml
summary_line: TLSv1.3
tags:
- Bots
- Spam Detection
- Contact Forms
- AI Classification
- Security
---
