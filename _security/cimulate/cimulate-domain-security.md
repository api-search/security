---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cimulate.ai
  spf: true
hosts:
- cert_expires: Oct  9 04:12:40 2026 GMT
  host: cimulate.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cimulate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cimulate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cimulate
provider_slug: cimulate
slug: cimulate-domain-security
source_filename: cimulate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cimulate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:12:40 2026 GMT\n  hsts: false\ndomains:\n- domain: cimulate.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cimulate/refs/heads/main/security/cimulate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Ecommerce
- Search
- Product Discovery
- Recommendations
- Agentic Commerce
- MCP
- Retail
- Conversational AI
---
