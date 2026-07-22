---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunarcrush.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunarcrush.ai
  spf: true
hosts:
- cert_expires: Sep  1 19:45:59 2026 GMT
  host: lunarcrush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:28:24 2026 GMT
  host: lunarcrush.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunarcrush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LunarCrush, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LunarCrush
provider_slug: lunarcrush
slug: lunarcrush-domain-security
source_filename: lunarcrush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunarcrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:45:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lunarcrush.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:28:24 2026 GMT\n  hsts: false\ndomains:\n- domain: lunarcrush.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lunarcrush.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunarcrush/refs/heads/main/security/lunarcrush-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Intelligence
- Cryptocurrency
- Stocks
- Sentiment Analysis
- Social Media
- Market Data
- Analytics
- AI Agents
- MCP
---
