---
api_specs:
- filename: innago-expenses-api-openapi.yml
  format: yaml
  label: Innago Expenses API
  slug: innago-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-expenses-api-openapi.yml
- filename: innago-external-references-api-openapi.yml
  format: yaml
  label: Innago External References API
  slug: innago-external-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-external-references-api-openapi.yml
- filename: innago-health-api-openapi.yml
  format: yaml
  label: Innago Health API
  slug: innago-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-health-api-openapi.yml
- filename: innago-invoices-api-openapi.yml
  format: yaml
  label: Innago Invoices API
  slug: innago-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-invoices-api-openapi.yml
- filename: innago-leases-api-openapi.yml
  format: yaml
  label: Innago Leases API
  slug: innago-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-leases-api-openapi.yml
- filename: innago-maintenance-api-openapi.yml
  format: yaml
  label: Innago Maintenance API
  slug: innago-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-maintenance-api-openapi.yml
- filename: innago-payments-api-openapi.yml
  format: yaml
  label: Innago Payments API
  slug: innago-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-payments-api-openapi.yml
- filename: innago-properties-api-openapi.yml
  format: yaml
  label: Innago Properties API
  slug: innago-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-properties-api-openapi.yml
- filename: innago-tenants-api-openapi.yml
  format: yaml
  label: Innago Tenants API
  slug: innago-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/innago-tenants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: innago.com
  spf: true
hosts:
- cert_expires: Oct  4 02:40:26 2026 GMT
  host: docs.innago.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: api-my.innago.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Innago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innago, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Innago
provider_slug: innago
slug: innago-domain-security
source_filename: innago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.innago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:40:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-my.innago.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: innago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/security/innago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Management
- Real-Estate
- Leases
- Rent Collection
- Maintenance
- Tenants
- Invoicing
- Payments
---
