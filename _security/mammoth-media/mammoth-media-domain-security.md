---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tokenbot.com
  spf: false
hosts:
- cert_expires: Oct  1 13:25:24 2026 GMT
  host: www.tokenbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 00:59:32 2026 GMT
  host: docs.tokenbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.tokenbot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mammoth Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mammoth Media, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mammoth Media
provider_slug: mammoth-media
slug: mammoth-media-domain-security
source_filename: mammoth-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tokenbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:25:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tokenbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:59:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tokenbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tokenbot.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"globalsign.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mammoth-media/refs/heads/main/security/mammoth-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Cryptocurrency
- Trading
- Copy Trading
- Fintech
- Webhooks
- MCP
- Developer Tools
- CLI
---
