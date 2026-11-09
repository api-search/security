---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cheapchat.tech
  spf: true
hosts:
- cert_expires: Dec 28 03:28:21 2026 GMT
  host: cheapchat.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cheapchat Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CheapChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CheapChat
provider_slug: cheapchat-tech
slug: cheapchat-tech-domain-security
source_filename: cheapchat-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheapchat.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 03:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cheapchat.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cheapchat-tech/security/cheapchat-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Messaging
- Instagram Automation
- Facebook Automation
- Comment to DM
- Visual Builder
- No-Code Automation
---
