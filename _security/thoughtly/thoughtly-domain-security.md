---
api_specs:
- filename: openapi.json
  format: json
  label: Thoughtly API
  slug: thoughtly-api
  spec_type: OpenAPI
  url: https://docs.thoughtly.com/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thoughtly.com
  spf: true
hosts:
- cert_expires: Sep 27 16:10:45 2026 GMT
  host: thoughtly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:08:11 2026 GMT
  host: docs.thoughtly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 06:05:13 2026 GMT
  host: api.thoughtly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thoughtly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thoughtly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thoughtly
provider_slug: thoughtly
slug: thoughtly-domain-security
source_filename: thoughtly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thoughtly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:10:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.thoughtly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:08:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.thoughtly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:05:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thoughtly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thoughtly/refs/heads/main/security/thoughtly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice AI
- Chat AI
- Conversational AI
- AI Agents
- Outbound Calling
- Inbound Calling
- Lead Conversion
- SMS
- WhatsApp
- CRM
- Telephony
---
