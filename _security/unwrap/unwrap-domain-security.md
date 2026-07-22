---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unwrap.ai
  spf: true
hosts:
- cert_expires: Oct 16 05:12:03 2026 GMT
  host: www.unwrap.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: docs.unwrap.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: data.api.production.unwrap.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unwrap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unwrap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unwrap
provider_slug: unwrap
slug: unwrap-domain-security
source_filename: unwrap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unwrap.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:12:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unwrap.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.api.production.unwrap.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unwrap.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unwrap/refs/heads/main/security/unwrap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Customer Feedback
- Customer Intelligence
- Product Analytics
- Voice of Customer
- NLP
- GraphQL
- MCP
---
