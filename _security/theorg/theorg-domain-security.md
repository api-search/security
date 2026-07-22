---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theorg.com
  spf: true
hosts:
- cert_expires: Sep 14 07:53:46 2026 GMT
  host: theorg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theorg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Org
provider_slug: theorg
slug: theorg-domain-security
source_filename: theorg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theorg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theorg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theorg/refs/heads/main/security/theorg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Organizational Charts
- People Data
- Sales Intelligence
- Prospecting
- Org Chart
- B2B Data
- MCP
---
