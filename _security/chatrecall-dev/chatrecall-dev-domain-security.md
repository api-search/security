---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chatrecall.dev
  spf: true
hosts:
- cert_expires: Jan  9 19:22:22 2027 GMT
  host: chatrecall.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: chat-recall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chat-recall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: chat-recall
provider_slug: chatrecall-dev
slug: chatrecall-dev-domain-security
source_filename: chatrecall-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatrecall.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 19:22:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chatrecall.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/chatrecall-dev/security/chatrecall-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Coding Assistants
- Developer Tools
- MCP
- Memory
- Search
- Secret Scanning
- Self-Hosted
- Open Source
---
