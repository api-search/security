---
api_specs:
- filename: mumo-chat-account-api-openapi.yml
  format: yaml
  label: mumo Account API
  slug: mumo-chat-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-account-api-openapi.yml
- filename: mumo-chat-deliberations-api-openapi.yml
  format: yaml
  label: mumo Deliberations API
  slug: mumo-chat-deliberations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-deliberations-api-openapi.yml
- filename: mumo-chat-sessions-api-openapi.yml
  format: yaml
  label: mumo Sessions API
  slug: mumo-chat-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-sessions-api-openapi.yml
- filename: mumo-chat-system-api-openapi.yml
  format: yaml
  label: mumo System API
  slug: mumo-chat-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mumo.chat
  spf: true
hosts:
- cert_expires: Jan 21 04:11:23 2027 GMT
  host: mumo.chat
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mumo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mumo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mumo
provider_slug: mumo-chat
slug: mumo-chat-domain-security
source_filename: mumo-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mumo.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 04:11:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mumo.chat\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mumo-chat/security/mumo-chat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Chatbots
- Multi-Model
- Collaboration
- OpenAI
---
