---
api_specs:
- filename: perk-cost-centers-api-openapi.yml
  format: yaml
  label: Perk Cost centers API
  slug: perk-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-cost-centers-api-openapi.yml
- filename: perk-custom-fields-api-openapi.yml
  format: yaml
  label: Perk Custom fields API
  slug: perk-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-custom-fields-api-openapi.yml
- filename: perk-bookings-api-openapi.yml
  format: yaml
  label: Perk Bookings API
  slug: perk-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-bookings-api-openapi.yml
- filename: perk-companies-api-openapi.yml
  format: yaml
  label: Perk Companies API
  slug: perk-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-companies-api-openapi.yml
- filename: perk-invoices-api-openapi.yml
  format: yaml
  label: Perk Invoices API
  slug: perk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-invoices-api-openapi.yml
- filename: perk-profiles-api-openapi.yml
  format: yaml
  label: Perk Profiles API
  slug: perk-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-profiles-api-openapi.yml
- filename: perk-schemas-api-openapi.yml
  format: yaml
  label: Perk Schemas API
  slug: perk-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-schemas-api-openapi.yml
- filename: perk-suppliers-api-openapi.yml
  format: yaml
  label: Perk Suppliers API
  slug: perk-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-suppliers-api-openapi.yml
- filename: perk-trips-api-openapi.yml
  format: yaml
  label: Perk Trips API
  slug: perk-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-trips-api-openapi.yml
- filename: perk-users-api-openapi.yml
  format: yaml
  label: Perk Users API
  slug: perk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-users-api-openapi.yml
- filename: perk-webhooks-api-openapi.yml
  format: yaml
  label: Perk Webhooks API
  slug: perk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-webhooks-api-openapi.yml
- filename: perk-resource-types-api-openapi.yml
  format: yaml
  label: Perk Resource Types API
  slug: perk-resource-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-resource-types-api-openapi.yml
- filename: perk-service-provider-config-api-openapi.yml
  format: yaml
  label: Perk Service Provider Config API
  slug: perk-service-provider-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-service-provider-config-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perk.com
  spf: true
hosts:
- cert_expires: Sep 28 19:54:20 2026 GMT
  host: developers.perk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.perk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: app.perk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Perk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perk
provider_slug: perk
slug: perk-domain-security
source_filename: perk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.perk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:54:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.perk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: app.perk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: perk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/security/perk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Corporate Travel
- Expense Management
- Spend Management
- Travel
- Invoices
- Fintech
- Software-as-a-Service
---
