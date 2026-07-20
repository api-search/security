---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chatfuel.com
  spf: true
hosts:
- cert_expires: Sep 12 16:33:47 2026 GMT
  host: chatfuel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 17:01:50 2026 GMT
  host: docs.chatfuel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 16:40:47 2026 GMT
  host: api.chatfuel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catnip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catnip, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Catnip
provider_slug: catnip
slug: catnip-domain-security
source_filename: catnip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatfuel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.chatfuel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chatfuel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:40:47 2026 GMT\n  hsts: null\ndomains:\n- domain: chatfuel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catnip/refs/heads/main/security/catnip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Chatbots
- Messaging
- Conversational AI
- Marketing Automation
- Facebook Messenger
- Instagram
- WhatsApp
- Customer Engagement
---
