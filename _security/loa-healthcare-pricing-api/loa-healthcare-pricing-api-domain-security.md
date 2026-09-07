---
api_specs:
- filename: loa-healthcare-pricing-api-entities-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entities API
  slug: loa-healthcare-pricing-api-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entities-api-openapi.yml
- filename: loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entity Analytics API
  slug: loa-healthcare-pricing-api-entity-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
- filename: loa-healthcare-pricing-api-entity-updates-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entity Updates API
  slug: loa-healthcare-pricing-api-entity-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entity-updates-api-openapi.yml
- filename: loa-healthcare-pricing-api-prices-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Prices API
  slug: loa-healthcare-pricing-api-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-prices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loacare.com
  spf: true
hosts:
- cert_expires: Nov  1 21:01:10 2026 GMT
  host: www.loacare.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loa Healthcare Pricing Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loa Healthcare Pricing API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loa Healthcare Pricing API
provider_slug: loa-healthcare-pricing-api
slug: loa-healthcare-pricing-api-domain-security
source_filename: loa-healthcare-pricing-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 21:01:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: loacare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/security/loa-healthcare-pricing-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Price Transparency
- medical pricing
- Hospitals
- Providers
- Provider Directory
- hospital prices
- CPT
- HCPCS
- MCP
- agent-native
- OpenAPI
- llms-txt
---
