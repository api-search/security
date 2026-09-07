---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abcoffee.in
  spf: true
hosts:
- cert_expires: Dec  3 18:10:31 2026 GMT
  host: abcoffee.in
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abcoffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abcoffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Abcoffee
provider_slug: abcoffee
slug: abcoffee-domain-security
source_filename: abcoffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abcoffee.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 18:10:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: abcoffee.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcoffee/refs/heads/main/security/abcoffee-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Coffee
- Food and Beverage
- Retail
- Commerce
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
- India
- Subscriptions
---
