---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goaichat.app
  spf: true
hosts:
- cert_expires: Dec 13 13:59:32 2026 GMT
  host: goaichat.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GO AI Chat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GO AI Chat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GO AI Chat
provider_slug: goaichat-app
slug: goaichat-app-domain-security
source_filename: goaichat-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goaichat.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 13:59:32 2026 GMT\n  hsts: false\ndomains:\n- domain: goaichat.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goaichat-app/security/goaichat-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Chatbots
- Image Generation
- Video Generation
- Multi-Modal
---
