---
api_specs:
- filename: servicetitan-crm-api-openapi.yml
  format: yaml
  label: ServiceTitan CRM API
  slug: servicetitan-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-crm-api-openapi.yml
- filename: servicetitan-jpm-api-openapi.yml
  format: yaml
  label: ServiceTitan Job Planning & Management API
  slug: servicetitan-jpm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-jpm-api-openapi.yml
- filename: servicetitan-dispatch-api-openapi.yml
  format: yaml
  label: ServiceTitan Dispatch API
  slug: servicetitan-dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-dispatch-api-openapi.yml
- filename: servicetitan-accounting-api-openapi.yml
  format: yaml
  label: ServiceTitan Accounting API
  slug: servicetitan-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-accounting-api-openapi.yml
- filename: servicetitan-pricebook-api-openapi.yml
  format: yaml
  label: ServiceTitan Pricebook API
  slug: servicetitan-pricebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-pricebook-api-openapi.yml
- filename: servicetitan-inventory-api-openapi.yml
  format: yaml
  label: ServiceTitan Inventory API
  slug: servicetitan-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-inventory-api-openapi.yml
- filename: servicetitan-equipment-systems-api-openapi.yml
  format: yaml
  label: ServiceTitan Equipment Systems API
  slug: servicetitan-equipment-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-equipment-systems-api-openapi.yml
- filename: servicetitan-settings-api-openapi.yml
  format: yaml
  label: ServiceTitan Settings API
  slug: servicetitan-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: servicetitan.io
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: servicetitan.com
  spf: true
hosts:
- cert_expires: Oct  3 09:57:38 2026 GMT
  host: developer.servicetitan.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:57:38 2026 GMT
  host: partnerapis.servicetitan.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 13:43:50 2026 GMT
  host: www.servicetitan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servicetitan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ServiceTitan, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: ServiceTitan
provider_slug: servicetitan
slug: servicetitan-domain-security
source_filename: servicetitan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.servicetitan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:57:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partnerapis.servicetitan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:57:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.servicetitan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 13:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: servicetitan.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: servicetitan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/security/servicetitan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Field Service Management
- Trades
- HVAC
- Plumbing
- Electrical
- Construction
- CRM
- Dispatch
- Accounting
- Pricebook
- Marketing
- Memberships
- Webhooks
---
