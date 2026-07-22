---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yalo.ai
  spf: false
hosts:
- cert_expires: Aug 23 07:52:41 2026 GMT
  host: www.yalo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yalo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yalo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Yalo
provider_slug: yalo
slug: yalo-domain-security
source_filename: yalo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yalo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:52:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yalo.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yalo/refs/heads/main/security/yalo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Conversational Commerce
- WhatsApp
- Messaging
- Sales
- Chat
- AI Agents
---
