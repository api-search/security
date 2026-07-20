---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bettermode.com
  spf: true
hosts:
- cert_expires: Sep 13 08:15:23 2026 GMT
  host: bettermode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bettermode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bettermode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bettermode
provider_slug: bettermode
slug: bettermode-domain-security
source_filename: bettermode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bettermode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:15:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bettermode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bettermode/refs/heads/main/security/bettermode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community
- Customer Community
- Community Platform
- Customer Engagement
- Customer Success
- GraphQL
- Webhooks
- No-Code
- SaaS
- Developer
---
