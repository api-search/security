---
api_specs:
- filename: papercups-openapi.yml
  format: yaml
  label: Papercups Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/openapi/papercups-openapi.yml
- filename: papercups-openapi.yml
  format: yaml
  label: Papercups Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/openapi/papercups-openapi.yml
- filename: papercups-openapi.yml
  format: yaml
  label: Papercups Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/openapi/papercups-openapi.yml
- filename: papercups-asyncapi.yml
  format: yaml
  label: Papercups Realtime Chat API (WebSocket / Phoenix Channels)
  slug: realtime-chat
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/asyncapi/papercups-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: papercups.io
  spf: true
hosts:
- cert_expires: Sep 20 16:07:46 2026 GMT
  host: papercups.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:16:32 2026 GMT
  host: docs.papercups.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: app.papercups.io
  https: false
kind: domain-security
layout: security
method: probed
name: Papercups Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Papercups, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Papercups
provider_slug: papercups
slug: papercups-domain-security
source_filename: papercups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: papercups.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:07:46 2026 GMT\n  hsts: null\n- host: docs.papercups.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:16:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.papercups.io\n  https: false\ndomains:\n- domain: papercups.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/security/papercups-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Messaging
- Live Chat
- Open Source
- Support
- Intercom Alternative
---
