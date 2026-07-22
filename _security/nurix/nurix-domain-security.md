---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nurix.ai
  spf: true
hosts:
- cert_expires: Sep 29 01:56:45 2026 GMT
  host: www.nurix.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nurix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nurix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nurix
provider_slug: nurix
slug: nurix-domain-security
source_filename: nurix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nurix.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:56:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nurix.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nurix/refs/heads/main/security/nurix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Agentic AI
- Customer Support
- Sales
- Voice
- Automation
- Contact Center
---
