---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: becausemarket.com
  spf: true
hosts:
- cert_expires: Aug 27 23:02:02 2026 GMT
  host: becausemarket.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Because Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Because, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Because
provider_slug: because
slug: because-domain-security
source_filename: because-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: becausemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:02:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: becausemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/because/refs/heads/main/security/because-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-commerce
- Health
- Incontinence
- Senior Care
- Agentic Commerce
- Shopify
---
