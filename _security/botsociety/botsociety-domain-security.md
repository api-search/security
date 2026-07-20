---
api_specs:
- filename: botsociety-openapi.yml
  format: yaml
  label: Botsociety API
  slug: botsociety-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botsociety/refs/heads/main/openapi/botsociety-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botsociety.io
  spf: true
hosts:
- cert_expires: Oct 16 00:00:44 2026 GMT
  host: botsociety.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Botsociety Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BotSociety, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BotSociety
provider_slug: botsociety
slug: botsociety-domain-security
source_filename: botsociety-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botsociety.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:00:44 2026 GMT\n  hsts: false\ndomains:\n- domain: botsociety.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botsociety/refs/heads/main/security/botsociety-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Chatbots
- Conversational AI
- Voice Assistants
- Bot Design
- Prototyping
- Developer Tools
---
