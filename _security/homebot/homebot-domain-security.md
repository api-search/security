---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homebot.ai
  spf: true
hosts:
- cert_expires: Oct 14 20:26:40 2026 GMT
  host: homebot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homebot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homebot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Homebot
provider_slug: homebot
slug: homebot-domain-security
source_filename: homebot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homebot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:26:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: homebot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homebot/refs/heads/main/security/homebot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Mortgage
- PropTech
- FinTech
- Homeownership
- Client Engagement
- CRM
- Lead Generation
- Webhooks
---
