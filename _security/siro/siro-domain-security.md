---
api_specs:
- filename: siro-external-api-openapi.json
  format: json
  label: Siro External API
  slug: siro-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-external-api-openapi.json
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
  dmarc_policy: none
  dnssec: true
  domain: siro.ai
  spf: true
hosts:
- cert_expires: Sep 12 05:45:56 2026 GMT
  host: siro.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 10:06:25 2026 GMT
  host: docs.siro.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:33:44 2026 GMT
  host: functions.siro.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Siro
provider_slug: siro
slug: siro-domain-security
source_filename: siro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:45:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.siro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:06:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: functions.siro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:33:44 2026 GMT\n  hsts: null\ndomains:\n- domain: siro.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/security/siro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- Sales Coaching
- Conversation Intelligence
- Field Sales
- CRM
- AI
- Speech to Text
- Webhooks
- Integrations
---
