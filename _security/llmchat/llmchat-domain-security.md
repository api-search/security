---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llmchat.co
  spf: false
hosts:
- cert_expires: Dec 31 06:03:38 2026 GMT
  host: llmchat.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLMChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LLMChat
provider_slug: llmchat
slug: llmchat-domain-security
source_filename: llmchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmchat.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:03:38 2026 GMT\n  hsts: null\ndomains:\n- domain: llmchat.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmchat/refs/heads/main/security/llmchat-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
