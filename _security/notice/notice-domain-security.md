---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notice.co
  spf: true
hosts:
- cert_expires: Oct 18 02:33:01 2026 GMT
  host: notice.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 02:33:01 2026 GMT
  host: learn.notice.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 02:33:01 2026 GMT
  host: api.notice.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notice, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Notice
provider_slug: notice
slug: notice-domain-security
source_filename: notice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notice.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 02:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: learn.notice.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 02:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.notice.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 02:33:01 2026 GMT\n  hsts: null\ndomains:\n- domain: notice.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notice/refs/heads/main/security/notice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Private Markets
- Market Data
- Financial Data
- Investing
- Pre-IPO
- Secondary Markets
- Valuations
- Fintech
- MCP
---
