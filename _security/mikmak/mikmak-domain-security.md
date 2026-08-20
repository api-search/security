---
api_specs:
- filename: mikmak-commerce-api-openapi.yml
  format: yaml
  label: MikMak Headless Commerce API
  slug: mikmak-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-commerce-api-openapi.yml
- filename: mikmak-insights-api-openapi.yml
  format: yaml
  label: MikMak Insights API
  slug: mikmak-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-insights-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mikmak.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mikmak.ai
  spf: false
hosts:
- cert_expires: Sep 20 05:38:49 2026 GMT
  host: www.mikmak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 00:47:23 2026 GMT
  host: docs.mikmak.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.mikmak.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mikmak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MikMak, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MikMak
provider_slug: mikmak
slug: mikmak-domain-security
source_filename: mikmak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mikmak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:38:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mikmak.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:47:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mikmak.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mikmak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mikmak.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/security/mikmak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Commerce
- E-Commerce
- Multi-Channel
- Retail Media
- Where to Buy
- Shoppable Media
- Product Availability
- MCP
- agent-native
- Reporting
- CPG
---
