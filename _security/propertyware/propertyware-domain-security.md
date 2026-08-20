---
api_specs:
- filename: propertyware-accounting-api-openapi.yml
  format: yaml
  label: Propertyware Accounting API
  slug: propertyware-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-accounting-api-openapi.yml
- filename: propertyware-bills-api-openapi.yml
  format: yaml
  label: Propertyware Bills API
  slug: propertyware-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-bills-api-openapi.yml
- filename: propertyware-buildings-api-openapi.yml
  format: yaml
  label: Propertyware Buildings API
  slug: propertyware-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-buildings-api-openapi.yml
- filename: propertyware-contacts-api-openapi.yml
  format: yaml
  label: Propertyware Contacts API
  slug: propertyware-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-contacts-api-openapi.yml
- filename: propertyware-custom-field-definitions-api-openapi.yml
  format: yaml
  label: Propertyware Custom field definitions API
  slug: propertyware-custom-field-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-custom-field-definitions-api-openapi.yml
- filename: propertyware-documents-api-openapi.yml
  format: yaml
  label: Propertyware Documents API
  slug: propertyware-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-documents-api-openapi.yml
- filename: propertyware-health-check-api-openapi.yml
  format: yaml
  label: Propertyware Health check API
  slug: propertyware-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-health-check-api-openapi.yml
- filename: propertyware-inspections-api-openapi.yml
  format: yaml
  label: Propertyware Inspections API
  slug: propertyware-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-inspections-api-openapi.yml
- filename: propertyware-leases-api-openapi.yml
  format: yaml
  label: Propertyware Leases API
  slug: propertyware-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-leases-api-openapi.yml
- filename: propertyware-portfolios-api-openapi.yml
  format: yaml
  label: Propertyware Portfolios API
  slug: propertyware-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-portfolios-api-openapi.yml
- filename: propertyware-prospects-api-openapi.yml
  format: yaml
  label: Propertyware Prospects API
  slug: propertyware-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-prospects-api-openapi.yml
- filename: propertyware-units-api-openapi.yml
  format: yaml
  label: Propertyware Units API
  slug: propertyware-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-units-api-openapi.yml
- filename: propertyware-vendors-api-openapi.yml
  format: yaml
  label: Propertyware Vendors API
  slug: propertyware-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-vendors-api-openapi.yml
- filename: propertyware-work-orders-api-openapi.yml
  format: yaml
  label: Propertyware Work orders API
  slug: propertyware-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-work-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: propertyware.com
  spf: true
hosts:
- cert_expires: Sep 29 10:46:27 2026 GMT
  host: www.propertyware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: app.propertyware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.propertyware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propertyware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propertyware, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Propertyware
provider_slug: propertyware
slug: propertyware-domain-security
source_filename: propertyware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propertyware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:46:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.propertyware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.propertyware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: propertyware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/security/propertyware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Management
- Real-Estate
- Rental Properties
- Single-Family Rentals
- Leases
- Tenants
- Maintenance
- Work Orders
- Financial Transactions
- Owner Reports
---
