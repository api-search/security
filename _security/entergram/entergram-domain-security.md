---
api_specs:
- filename: entergram-openapi.json
  format: json
  label: Entergram API
  slug: entergram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: entergram.com
  spf: true
hosts:
- cert_expires: Nov  2 15:17:44 2026 GMT
  host: api.entergram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entergram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entergram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Entergram
provider_slug: entergram
slug: entergram-domain-security
source_filename: entergram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.entergram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 15:17:44 2026 GMT\n  hsts: null\ndomains:\n- domain: entergram.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/security/entergram-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Messaging
- Notifications
- Communications
- CRM
- Telegram
- Customer Support
- Ticketing
- Sales
- MCP
- Webhooks
---
