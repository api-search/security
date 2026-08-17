---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spate.nyc
  spf: true
hosts:
- cert_expires: Oct 26 07:26:22 2026 GMT
  host: spate.nyc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: help.spate.nyc
  hsts: true
  hsts_max_age: 30
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 16:50:11 2026 GMT
  host: api.spate.nyc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spate
provider_slug: spate
slug: spate-domain-security
source_filename: spate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spate.nyc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 07:26:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.spate.nyc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 30\n- host: api.spate.nyc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:50:11 2026 GMT\n  hsts: null\ndomains:\n- domain: spate.nyc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spate/refs/heads/main/security/spate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Market Intelligence
- Trend Forecasting
- Consumer Insights
- Social Listening
- Analytics
- Beauty
- MCP
- AI Agents
- Trend Data
- Consumer Packaged Goods
---
