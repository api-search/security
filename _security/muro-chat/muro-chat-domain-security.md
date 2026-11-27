---
api_specs:
- filename: muro-chat-ai-api-openapi.yml
  format: yaml
  label: muro AI API
  slug: muro-chat-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-ai-api-openapi.yml
- filename: muro-chat-automation-api-openapi.yml
  format: yaml
  label: muro Automation API
  slug: muro-chat-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-automation-api-openapi.yml
- filename: muro-chat-contacts-api-openapi.yml
  format: yaml
  label: muro Contacts API
  slug: muro-chat-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-contacts-api-openapi.yml
- filename: muro-chat-conversations-api-openapi.yml
  format: yaml
  label: muro Conversations API
  slug: muro-chat-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-conversations-api-openapi.yml
- filename: muro-chat-messages-api-openapi.yml
  format: yaml
  label: muro Messages API
  slug: muro-chat-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-messages-api-openapi.yml
- filename: muro-chat-meta-api-openapi.yml
  format: yaml
  label: muro Meta API
  slug: muro-chat-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-meta-api-openapi.yml
- filename: muro-chat-realtime-api-openapi.yml
  format: yaml
  label: muro Realtime API
  slug: muro-chat-realtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-realtime-api-openapi.yml
- filename: muro-chat-saved-replies-api-openapi.yml
  format: yaml
  label: muro Saved replies API
  slug: muro-chat-saved-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-saved-replies-api-openapi.yml
- filename: muro-chat-sites-api-openapi.yml
  format: yaml
  label: muro Sites API
  slug: muro-chat-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-sites-api-openapi.yml
- filename: muro-chat-webhooks-api-openapi.yml
  format: yaml
  label: muro Webhooks API
  slug: muro-chat-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muro-chat/openapi/muro-chat-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: muro.chat
  spf: true
hosts:
- cert_expires: Jan 27 05:12:03 2027 GMT
  host: muro.chat
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: muro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for muro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: muro
provider_slug: muro-chat
slug: muro-chat-domain-security
source_filename: muro-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: muro.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 05:12:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: muro.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/muro-chat/security/muro-chat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Live Chat
- Agency
- Resell
- Software-as-a-Service
---
