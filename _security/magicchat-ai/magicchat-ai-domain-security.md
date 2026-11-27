---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: magicchat.ai
  spf: false
hosts:
- cert_expires: Jan  1 13:13:48 2027 GMT
  host: magicchat.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MagicChat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MagicChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MagicChat
provider_slug: magicchat-ai
slug: magicchat-ai-domain-security
source_filename: magicchat-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magicchat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 13:13:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: magicchat.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/magicchat-ai/security/magicchat-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Customer Service
- Chatbots
- Software-as-a-Service
- MagicChat
---
