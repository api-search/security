---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carapace.bot
  spf: false
hosts:
- cert_expires: Jan  1 05:51:07 2027 GMT
  host: carapace.bot
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carapace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carapace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Carapace
provider_slug: carapace-bot
slug: carapace-bot-domain-security
source_filename: carapace-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carapace.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:51:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carapace.bot\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/carapace-bot/security/carapace-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Secrets Management
- Confidential Computing
- Security
- Open Source
- Google Cloud
- Self-Hosted
---
