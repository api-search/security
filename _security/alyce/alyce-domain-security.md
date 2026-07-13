---
api_specs:
- filename: api
  format: yaml
  label: Alyce API
  slug: alyce-api
  spec_type: OpenAPI
  url: https://app.alyce.com/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alyce.com
  spf: true
hosts:
- host: www.alyce.com
  https: false
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: help.alyce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: app.alyce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Alyce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alyce, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alyce
provider_slug: alyce
slug: alyce-domain-security
source_filename: alyce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alyce.com\n  https: false\n- host: help.alyce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: app.alyce.com\n  https: false\ndomains:\n- domain: alyce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alyce/refs/heads/main/security/alyce-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gifting
- Corporate Gifting
- B2B
- Marketing Automation
- CRM Integration
- Account-Based Marketing
- Sales Enablement
- AI
- Personalization
- Direct Mail
---
