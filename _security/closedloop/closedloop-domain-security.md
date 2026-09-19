---
api_specs:
- filename: closedloop-analytics-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Analytics API
  slug: closedloop-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-analytics-api-openapi.yml
- filename: closedloop-competitors-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Competitors API
  slug: closedloop-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-competitors-api-openapi.yml
- filename: closedloop-context-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Context API
  slug: closedloop-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-context-api-openapi.yml
- filename: closedloop-customers-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Customers API
  slug: closedloop-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-customers-api-openapi.yml
- filename: closedloop-features-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Features API
  slug: closedloop-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-features-api-openapi.yml
- filename: closedloop-insights-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Insights API
  slug: closedloop-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-insights-api-openapi.yml
- filename: closedloop-integrations-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Integrations API
  slug: closedloop-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-integrations-api-openapi.yml
- filename: closedloop-meta-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Meta API
  slug: closedloop-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-meta-api-openapi.yml
- filename: closedloop-products-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Products API
  slug: closedloop-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-products-api-openapi.yml
- filename: closedloop-themes-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Themes API
  slug: closedloop-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-themes-api-openapi.yml
- filename: closedloop-usage-api-openapi.yml
  format: yaml
  label: ClosedLoop AI Usage API
  slug: closedloop-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: closedloop.sh
  spf: true
hosts:
- cert_expires: Oct  1 08:57:43 2026 GMT
  host: docs.closedloop.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 08:57:43 2026 GMT
  host: api.closedloop.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 08:57:43 2026 GMT
  host: closedloop.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Closedloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClosedLoop AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ClosedLoop AI
provider_slug: closedloop
slug: closedloop-domain-security
source_filename: closedloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.closedloop.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:57:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.closedloop.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:57:43 2026 GMT\n  hsts: null\n- host: closedloop.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:57:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: closedloop.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/security/closedloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Intelligence
- Customer Feedback
- Voice of Customer
- Product Management
- Agentic AI
- MCP
- SaaS analytics
- A2A
- SCIM
- Product Discovery
---
