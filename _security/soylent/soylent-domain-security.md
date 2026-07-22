---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soylent.com
  spf: true
hosts:
- cert_expires: Aug 27 19:00:02 2026 GMT
  host: soylent.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soylent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soylent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Soylent
provider_slug: soylent
slug: soylent-domain-security
source_filename: soylent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soylent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:00:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: soylent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soylent/refs/heads/main/security/soylent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Nutrition
- Food and Beverage
- Meal Replacement
- Ecommerce
- Retail
- Direct-to-Consumer
- Agent Commerce
- Universal Commerce Protocol
- Shopify
- MCP
---
