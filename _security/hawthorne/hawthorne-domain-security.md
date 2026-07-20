---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hawthorne.co
  spf: true
hosts:
- cert_expires: Aug 24 14:17:32 2026 GMT
  host: hawthorne.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hawthorne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hawthorne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hawthorne
provider_slug: hawthorne
slug: hawthorne-domain-security
source_filename: hawthorne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hawthorne.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:17:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hawthorne.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawthorne/refs/heads/main/security/hawthorne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Consumer Goods
- Personal Care
- Grooming
- Agentic Commerce
- Shopify
---
