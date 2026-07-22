---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: primeroots.com
  spf: true
hosts:
- cert_expires: Aug 30 09:26:02 2026 GMT
  host: primeroots.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prime Roots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prime Roots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Prime Roots
provider_slug: prime-roots
slug: prime-roots-domain-security
source_filename: prime-roots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: primeroots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 09:26:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: primeroots.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-roots/refs/heads/main/security/prime-roots-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Foodtech
- Plant-Based
- Deli Meat
- Food Service
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Ecommerce
---
