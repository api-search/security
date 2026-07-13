---
api_specs:
- filename: swagger.json
  format: json
  label: Chatwoot Application API
  slug: application-api
  spec_type: OpenAPI
  url: https://www.chatwoot.com/swagger/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chatwoot.com
  spf: true
hosts:
- cert_expires: Sep 21 09:14:14 2026 GMT
  host: www.chatwoot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 13:04:31 2026 GMT
  host: developers.chatwoot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: app.chatwoot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chatwoot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatwoot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chatwoot
provider_slug: chatwoot
slug: chatwoot-domain-security
source_filename: chatwoot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chatwoot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.chatwoot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:04:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.chatwoot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: chatwoot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatwoot/refs/heads/main/security/chatwoot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Messaging
- Live Chat
- Omni-channel
- Conversations
- Contacts
- Agents
- Open Source
---
