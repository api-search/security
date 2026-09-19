---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agnikul.in
  spf: true
hosts:
- cert_expires: Oct 29 17:48:19 2026 GMT
  host: agnikul.in
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 04:43:01 2026 GMT
  host: shop.agnikul.in
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agnikul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agnikul Cosmos, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agnikul Cosmos
provider_slug: agnikul
slug: agnikul-domain-security
source_filename: agnikul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agnikul.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:48:19 2026 GMT\n  hsts: false\n- host: shop.agnikul.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 04:43:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: agnikul.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agnikul/refs/heads/main/security/agnikul-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Aerospace
- Space
- Launch Services
- Satellite
- Manufacturing
- Additive Manufacturing
- India
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
