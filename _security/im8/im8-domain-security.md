---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: im8health.com
  spf: true
hosts:
- cert_expires: Sep  5 09:55:31 2026 GMT
  host: im8health.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Im8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IM8 Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IM8 Health
provider_slug: im8
slug: im8-domain-security
source_filename: im8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: im8health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:55:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: im8health.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/im8/refs/heads/main/security/im8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Wellness
- Supplements
- Nutrition
- Ecommerce
- Direct-to-Consumer
- Agentic Commerce
- Shopify
- UCP
- MCP
---
