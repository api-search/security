---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nooks.ai
  spf: true
hosts:
- cert_expires: Sep  8 20:01:13 2026 GMT
  host: www.nooks.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nooks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nooks
provider_slug: nooks
slug: nooks-domain-security
source_filename: nooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nooks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:01:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nooks.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/security/nooks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Sales Engagement
- Sales Dialer
- AI SDR
- Outbound Sales
- Sales Coaching
- Revenue Operations
---
