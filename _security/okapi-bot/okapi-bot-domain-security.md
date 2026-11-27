---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: okapi.bot
  spf: true
hosts:
- cert_expires: Jan 17 08:18:56 2027 GMT
  host: www.okapi.bot
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Okapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okapi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Okapi
provider_slug: okapi-bot
slug: okapi-bot-domain-security
source_filename: okapi-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.okapi.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 08:18:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: okapi.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/okapi-bot/security/okapi-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Change Management
- Breaking Changes
- Deprecation
- GitHub App
- Developer Tools
- API Monitoring
- AI Agents
---
