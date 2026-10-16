---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chatpromptgenius.com
  spf: true
hosts:
- cert_expires: Dec 12 10:13:55 2026 GMT
  host: chatpromptgenius.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chatpromptgenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chat Prompt Genius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chat Prompt Genius
provider_slug: chatpromptgenius
slug: chatpromptgenius-domain-security
source_filename: chatpromptgenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatpromptgenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 10:13:55 2026 GMT\n  hsts: false\ndomains:\n- domain: chatpromptgenius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatpromptgenius/refs/heads/main/security/chatpromptgenius-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- PromptMarketplace
- Marketing
- ECommerce
---
