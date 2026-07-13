---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: botpress.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botpress.cloud
  spf: true
hosts:
- cert_expires: Sep 22 08:21:07 2026 GMT
  host: botpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.botpress.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: chat.botpress.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Botpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botpress, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Botpress
provider_slug: botpress
slug: botpress-domain-security
source_filename: botpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.botpress.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\n- host: chat.botpress.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: botpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: botpress.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/security/botpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Conversational
- Chat
- Open Source
- Bot Builder
- LLM
---
