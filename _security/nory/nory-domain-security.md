---
api_specs:
- filename: nory-authorization-api-openapi.yml
  format: yaml
  label: Nory Authorization API
  slug: nory-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-authorization-api-openapi.yml
- filename: nory-branch-api-openapi.yml
  format: yaml
  label: Nory Branch API
  slug: nory-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-branch-api-openapi.yml
- filename: nory-brands-api-openapi.yml
  format: yaml
  label: Nory Brands API
  slug: nory-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-brands-api-openapi.yml
- filename: nory-employee-punch-api-openapi.yml
  format: yaml
  label: Nory Employee Punch API
  slug: nory-employee-punch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-employee-punch-api-openapi.yml
- filename: nory-integration-api-openapi.yml
  format: yaml
  label: Nory Integration API
  slug: nory-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-integration-api-openapi.yml
- filename: nory-inventory-api-openapi.yml
  format: yaml
  label: Nory Inventory API
  slug: nory-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-inventory-api-openapi.yml
- filename: nory-inventory-orders-api-openapi.yml
  format: yaml
  label: Nory Inventory Orders API
  slug: nory-inventory-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-inventory-orders-api-openapi.yml
- filename: nory-location-settings-api-openapi.yml
  format: yaml
  label: Nory Location Settings API
  slug: nory-location-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-location-settings-api-openapi.yml
- filename: nory-refresh-token-api-openapi.yml
  format: yaml
  label: Nory Refresh token API
  slug: nory-refresh-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-refresh-token-api-openapi.yml
- filename: nory-templates-api-openapi.yml
  format: yaml
  label: Nory Templates API
  slug: nory-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nory.ai
  spf: true
hosts:
- cert_expires: Sep 13 15:10:28 2026 GMT
  host: nory.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nory
provider_slug: nory
slug: nory-domain-security
source_filename: nory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:10:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nory.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/security/nory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurant
- Hospitality
- Inventory
- Workforce
- Payroll
- Point-of-Sale
- Artificial Intelligence
- Food and Beverage
---
