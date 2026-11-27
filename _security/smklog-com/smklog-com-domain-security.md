---
api_specs:
- filename: smklog-com-operations-api-openapi.yml
  format: yaml
  label: SMKlog Operations API
  slug: smklog-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-operations-api-openapi.yml
- filename: smklog-com-dimensional-weight-api-openapi.yml
  format: yaml
  label: SMKlog Dimensional Weight API
  slug: smklog-com-dimensional-weight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-dimensional-weight-api-openapi.yml
- filename: smklog-com-holiday-shipping-api-openapi.yml
  format: yaml
  label: SMKlog Holiday Shipping API
  slug: smklog-com-holiday-shipping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-holiday-shipping-api-openapi.yml
- filename: smklog-com-payments-api-openapi.yml
  format: yaml
  label: SMKlog Payments API
  slug: smklog-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-payments-api-openapi.yml
- filename: smklog-com-price-index-api-openapi.yml
  format: yaml
  label: SMKlog Price Index API
  slug: smklog-com-price-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-price-index-api-openapi.yml
- filename: smklog-com-refunds-api-openapi.yml
  format: yaml
  label: SMKlog Refunds API
  slug: smklog-com-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-refunds-api-openapi.yml
- filename: smklog-com-shipping-rates-api-openapi.yml
  format: yaml
  label: SMKlog Shipping Rates API
  slug: smklog-com-shipping-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-shipping-rates-api-openapi.yml
- filename: smklog-com-shipping-restrictions-api-openapi.yml
  format: yaml
  label: SMKlog Shipping Restrictions API
  slug: smklog-com-shipping-restrictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-shipping-restrictions-api-openapi.yml
- filename: smklog-com-tracking-api-openapi.yml
  format: yaml
  label: SMKlog Tracking API
  slug: smklog-com-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-tracking-api-openapi.yml
- filename: smklog-com-webhooks-api-openapi.yml
  format: yaml
  label: SMKlog Webhooks API
  slug: smklog-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smklog-com/openapi/smklog-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: smklog.com
  spf: true
hosts:
- cert_expires: Nov 20 02:45:24 2026 GMT
  host: smklog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 21:27:59 2026 GMT
  host: quote-api.smklog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: SMKlog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMKlog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SMKlog
provider_slug: smklog-com
slug: smklog-com-domain-security
source_filename: smklog-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smklog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:45:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: quote-api.smklog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 21:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: smklog.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/smklog-com/security/smklog-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Shipping
- Logistics
- Parcel Shipping
- shipping-rates
- Shipping Labels
- E-Commerce
- Agents
- MCP
- A2A
---
