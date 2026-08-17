---
api_specs:
- filename: replyrai-platform-api-swagger.json
  format: json
  label: Replyr Platform API
  slug: replyr-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/openapi/replyrai-platform-api-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: replyr.ai
  spf: false
hosts:
- cert_expires: Oct 27 10:32:53 2026 GMT
  host: replyr.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 00:22:18 2026 GMT
  host: app.replyr.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replyrai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replyr.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Replyr.ai
provider_slug: replyrai
slug: replyrai-domain-security
source_filename: replyrai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: replyr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 10:32:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.replyr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:22:18 2026 GMT\n  hsts: false\ndomains:\n- domain: replyr.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replyrai/refs/heads/main/security/replyrai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Chatbots
- Conversational AI
- Customer Engagement
- Lead Generation
- WhatsApp
- Marketing
- Messaging
- CRM
- Appointment Scheduling
- Healthcare
- Malaysia
---
