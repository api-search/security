---
api_specs:
- filename: intelligems-analytics-api-openapi.yml
  format: yaml
  label: Intelligems Analytics API
  slug: intelligems-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-analytics-api-openapi.yml
- filename: intelligems-experiences-api-openapi.yml
  format: yaml
  label: Intelligems Experiences API
  slug: intelligems-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-experiences-api-openapi.yml
- filename: intelligems-holiday-benchmark-api-openapi.yml
  format: yaml
  label: Intelligems Holiday Benchmark API
  slug: intelligems-holiday-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-holiday-benchmark-api-openapi.yml
- filename: intelligems-custom-events-api-openapi.yml
  format: yaml
  label: Intelligems Custom Events API
  slug: intelligems-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-custom-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intelligems.io
  spf: true
hosts:
- cert_expires: Sep 28 08:16:39 2026 GMT
  host: intelligems.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 15:00:30 2026 GMT
  host: docs.intelligems.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.intelligems.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intelligems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intelligems, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Intelligems
provider_slug: intelligems
slug: intelligems-domain-security
source_filename: intelligems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intelligems.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.intelligems.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 15:00:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.intelligems.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: intelligems.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/security/intelligems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- A/B Testing
- E-Commerce
- Pricing
- Personalization
- Conversion Rate Optimization
- Shopify
- Analytics
- Experimentation
- MCP
- Webhook
- Profit Optimization
---
