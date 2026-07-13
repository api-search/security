---
api_specs:
- filename: groove-openapi.yml
  format: yaml
  label: Groove REST API v1
  slug: rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-openapi.yml
- filename: groove-webhooks-asyncapi.yml
  format: yaml
  label: Groove Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/asyncapi/groove-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groovehq.com
  spf: true
hosts:
- cert_expires: Aug 16 01:25:20 2026 GMT
  host: www.groovehq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: developer.groovehq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.groovehq.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Groove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groove, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Groove
provider_slug: groove
slug: groove-domain-security
source_filename: groove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.groovehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 01:25:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.groovehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.groovehq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: groovehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/security/groove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Helpdesk
- Shared Inbox
- Knowledge Base
- Conversations
- Live Chat
---
