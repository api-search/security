---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: junocompanion.com
  spf: true
hosts:
- cert_expires: Oct  1 06:14:59 2026 GMT
  host: junocompanion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juno Chat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juno Chat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Juno Chat
provider_slug: juno-chat
slug: juno-chat-domain-security
source_filename: juno-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: junocompanion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:14:59 2026 GMT\n  hsts: null\ndomains:\n- domain: junocompanion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juno-chat/refs/heads/main/security/juno-chat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Health
- Chronic Illness
- AI Health Assistant
- Symptom Tracking
- Consumer Health
- Mobile App
- Y Combinator
---
