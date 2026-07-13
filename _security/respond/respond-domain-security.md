---
api_specs:
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Comments API
  slug: comments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Tags and Custom Fields API
  slug: tags-custom-fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: respond.io
  spf: true
hosts:
- cert_expires: Sep 30 19:09:53 2026 GMT
  host: respond.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 18:31:07 2026 GMT
  host: developers.respond.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.respond.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Respond Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Respond.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Respond.io
provider_slug: respond
slug: respond-domain-security
source_filename: respond-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: respond.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:09:53 2026 GMT\n  hsts: false\n- host: developers.respond.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:31:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.respond.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: respond.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/security/respond-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Omnichannel
- Customer Conversations
- WhatsApp
- AI
---
