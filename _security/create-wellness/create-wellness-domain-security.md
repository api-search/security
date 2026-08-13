---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trycreate.co
  spf: true
hosts:
- cert_expires: Nov  8 16:20:34 2026 GMT
  host: trycreate.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Create Wellness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Create Wellness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Create Wellness
provider_slug: create-wellness
slug: create-wellness-domain-security
source_filename: create-wellness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trycreate.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 16:20:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: trycreate.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/create-wellness/refs/heads/main/security/create-wellness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health and Wellness
- Supplements
- Consumer Products
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- MCP
- Shopify
- Nutrition
---
