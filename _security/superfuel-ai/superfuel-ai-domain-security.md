---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superfuel.io
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: superfuel.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superfuel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superfuel AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superfuel AI
provider_slug: superfuel-ai
slug: superfuel-ai-domain-security
source_filename: superfuel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superfuel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: superfuel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superfuel-ai/refs/heads/main/security/superfuel-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ecommerce
- Amazon
- Amazon Sellers
- Listing Optimization
- AI Agent
- Workflows
- SaaS
---
