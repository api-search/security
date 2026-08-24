---
api_specs:
- filename: happy-cabbage-analytics-happy-buyers-external-openapi.yml
  format: yaml
  label: Happy Buyers External API
  slug: happy-buyers-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-happy-buyers-external-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: happycabbage.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: cabbage.pub
  spf: false
hosts:
- cert_expires: Oct 15 18:07:54 2026 GMT
  host: www.happycabbage.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 04:12:51 2026 GMT
  host: cabbage.pub
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 17:28:22 2026 GMT
  host: api.happycabbage.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Happy Cabbage Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Happy Cabbage Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Happy Cabbage Analytics
provider_slug: happy-cabbage-analytics
slug: happy-cabbage-analytics-domain-security
source_filename: happy-cabbage-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.happycabbage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:07:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cabbage.pub\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:12:51 2026 GMT\n  hsts: null\n- host: api.happycabbage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 17:28:22 2026 GMT\n  hsts: null\ndomains:\n- domain: happycabbage.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cabbage.pub\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/security/happy-cabbage-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cannabis
- Retail
- Inventory Management
- Analytics
- Purchasing
- Point of Sale
- Wholesale
- Demand Forecasting
- Supply Chain
- agent-native
---
