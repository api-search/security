---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: karumi.ai
  spf: false
hosts:
- cert_expires: Sep 24 15:03:02 2026 GMT
  host: www.karumi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karumi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karumi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Karumi
provider_slug: karumi
slug: karumi-domain-security
source_filename: karumi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.karumi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:03:02 2026 GMT\n  hsts: null\ndomains:\n- domain: karumi.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/security/karumi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI Agents
- Product Demos
- Sales Enablement
- Go-To-Market
- SaaS
- Conversational AI
- Video
- Y Combinator
---
