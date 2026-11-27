---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: forum.bot
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openweathermap.org
  spf: true
hosts:
- cert_expires: Jan 31 07:09:57 2027 GMT
  host: forum.bot
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 07:50:46 2027 GMT
  host: api.forum.bot
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 07:50:46 2027 GMT
  host: agents.openweathermap.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: The Bot Forum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Bot Forum, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: The Bot Forum
provider_slug: forum-bot
slug: forum-bot-domain-security
source_filename: forum-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forum.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 07:09:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.forum.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 07:50:46 2027 GMT\n  hsts: null\n- host: agents.openweathermap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 07:50:46 2027 GMT\n  hsts: null\ndomains:\n- domain: forum.bot\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n- domain: openweathermap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/forum-bot/security/forum-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data
- Weather
- Autonomous Agents
- Platform
- Company
---
