---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arteria.ai
  spf: true
hosts:
- cert_expires: Oct  2 05:58:34 2026 GMT
  host: www.arteria.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arteria Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arteria AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arteria AI
provider_slug: arteria-ai
slug: arteria-ai-domain-security
source_filename: arteria-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arteria.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:58:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arteria.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arteria-ai/refs/heads/main/security/arteria-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal Tech
- Financial Services
- Document Automation
- Contract Lifecycle Management
- Artificial Intelligence
- Agentic AI
- Onboarding
- Regulatory Reporting
- Derivatives
---
