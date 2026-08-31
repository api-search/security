---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yana.ai
  spf: false
hosts:
- cert_expires: Aug 27 00:15:43 2026 GMT
  host: yana.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Yana
provider_slug: yana
slug: yana-domain-security
source_filename: yana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:15:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yana.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yana/refs/heads/main/security/yana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mental Health
- Emotional Wellness
- AI Companion
- Chatbot
- Mobile Apps
- Consumer
---
