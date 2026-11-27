---
api_specs:
- filename: meet-bot-api-v1-api-openapi.yml
  format: yaml
  label: Meet.bot API v1 API
  slug: meet-bot-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meet-bot/openapi/meet-bot-api-v1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meet.bot
  spf: true
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: meet.bot
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meet.bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meet.bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meet.bot
provider_slug: meet-bot
slug: meet-bot-domain-security
source_filename: meet-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meet.bot\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: meet.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/meet-bot/security/meet-bot-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Scheduling
- AI Agents
- Integration
- Meetings
- Automation
---
