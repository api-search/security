---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: couple.me
  spf: false
hosts:
- cert_expires: Sep 28 11:49:19 2026 GMT
  host: couple.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Couple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for couple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: couple
provider_slug: couple
slug: couple-domain-security
source_filename: couple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: couple.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:49:19 2026 GMT\n  hsts: false\ndomains:\n- domain: couple.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/couple/refs/heads/main/security/couple-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Companion
- Chatbot
- Conversational AI
- Consumer
- Entertainment
---
