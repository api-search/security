---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mophones.co
  spf: true
hosts:
- cert_expires: Sep  8 16:44:34 2026 GMT
  host: mophones.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mophones Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mophones, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mophones
provider_slug: mophones
slug: mophones-domain-security
source_filename: mophones-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mophones.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:44:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mophones.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mophones/refs/heads/main/security/mophones-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Fintech
- Recommerce
- Africa
---
