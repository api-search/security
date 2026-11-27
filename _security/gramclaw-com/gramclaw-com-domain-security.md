---
api_specs:
- filename: gramclaw-com-api-openapi.json
  format: json
  label: GramClaw Telegram API API
  slug: gramclaw-telegram-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gramclaw-com/openapi/_original/gramclaw-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gramclaw.com
  spf: false
hosts:
- cert_expires: Feb  7 12:30:47 2027 GMT
  host: gramclaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GramClaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GramClaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: GramClaw
provider_slug: gramclaw-com
slug: gramclaw-com-domain-security
source_filename: gramclaw-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gramclaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 12:30:47 2027 GMT\n  hsts: false\ndomains:\n- domain: gramclaw.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gramclaw-com/security/gramclaw-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telegram
- Outreach
- Marketing
- Automation
- MCP
---
