---
api_specs:
- filename: chatbase-chat-api-openapi.yml
  format: yaml
  label: Chatbase Chat API
  slug: chatbase-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-chat-api-openapi.yml
- filename: chatbase-chatbots-api-openapi.yml
  format: yaml
  label: Chatbase Chatbots API
  slug: chatbase-chatbots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-chatbots-api-openapi.yml
- filename: chatbase-contacts-api-openapi.yml
  format: yaml
  label: Chatbase Contacts API
  slug: chatbase-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-contacts-api-openapi.yml
- filename: chatbase-conversations-api-openapi.yml
  format: yaml
  label: Chatbase Conversations API
  slug: chatbase-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-conversations-api-openapi.yml
- filename: chatbase-leads-api-openapi.yml
  format: yaml
  label: Chatbase Leads API
  slug: chatbase-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-leads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chatbase.co
  spf: true
hosts:
- cert_expires: Sep 18 03:49:34 2026 GMT
  host: www.chatbase.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chatbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatbase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chatbase
provider_slug: chatbase
slug: chatbase-domain-security
source_filename: chatbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chatbase.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:49:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chatbase.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/security/chatbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Chatbot
- AI Agent
- Customer Support
- Conversational AI
---
