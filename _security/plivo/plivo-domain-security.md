---
api_specs:
- filename: plivo-asyncapi.yml
  format: yaml
  label: Plivo Audio Stream API
  slug: plivo-audio-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/plivo/refs/heads/main/asyncapi/plivo-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plivo.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: www.plivo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.plivo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Plivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plivo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plivo
provider_slug: plivo
slug: plivo-domain-security
source_filename: plivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.plivo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: plivo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plivo/refs/heads/main/security/plivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- CPaaS
- Voice
- SMS
- Messaging
- WhatsApp
- SIP Trunking
- Verify
---
