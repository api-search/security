---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skippr.com
  spf: true
hosts:
- cert_expires: Sep 15 19:41:47 2026 GMT
  host: skippr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skippr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skippr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skippr
provider_slug: skippr
slug: skippr-domain-security
source_filename: skippr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skippr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:41:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: skippr.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skippr/refs/heads/main/security/skippr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- AI Agents
- Voice Agents
- Developer Tools
- MCP
- SDK
- Product Analytics
- Accessibility
---
