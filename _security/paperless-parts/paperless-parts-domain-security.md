---
api_specs:
- filename: paperless-parts-contacts-api-openapi.yml
  format: yaml
  label: Paperless Parts Contacts API
  slug: paperless-parts-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-contacts-api-openapi.yml
- filename: paperless-parts-custom-tables-api-openapi.yml
  format: yaml
  label: Paperless Parts Custom Tables API
  slug: paperless-parts-custom-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-custom-tables-api-openapi.yml
- filename: paperless-parts-customers-api-openapi.yml
  format: yaml
  label: Paperless Parts Customers API
  slug: paperless-parts-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-customers-api-openapi.yml
- filename: paperless-parts-events-api-openapi.yml
  format: yaml
  label: Paperless Parts Events API
  slug: paperless-parts-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-events-api-openapi.yml
- filename: paperless-parts-integration-actions-api-openapi.yml
  format: yaml
  label: Paperless Parts Integration Actions API
  slug: paperless-parts-integration-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-integration-actions-api-openapi.yml
- filename: paperless-parts-jobs-api-openapi.yml
  format: yaml
  label: Paperless Parts Jobs API
  slug: paperless-parts-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-jobs-api-openapi.yml
- filename: paperless-parts-orders-api-openapi.yml
  format: yaml
  label: Paperless Parts Orders API
  slug: paperless-parts-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-orders-api-openapi.yml
- filename: paperless-parts-parts-api-openapi.yml
  format: yaml
  label: Paperless Parts Parts API
  slug: paperless-parts-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-parts-api-openapi.yml
- filename: paperless-parts-processes-api-openapi.yml
  format: yaml
  label: Paperless Parts Processes API
  slug: paperless-parts-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-processes-api-openapi.yml
- filename: paperless-parts-purchased-components-api-openapi.yml
  format: yaml
  label: Paperless Parts Purchased Components API
  slug: paperless-parts-purchased-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-purchased-components-api-openapi.yml
- filename: paperless-parts-quote-items-api-openapi.yml
  format: yaml
  label: Paperless Parts Quote Items API
  slug: paperless-parts-quote-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-quote-items-api-openapi.yml
- filename: paperless-parts-quotes-api-openapi.yml
  format: yaml
  label: Paperless Parts Quotes API
  slug: paperless-parts-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-quotes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: paperlessparts.com
  spf: true
hosts:
- cert_expires: Nov 13 09:00:12 2026 GMT
  host: www.paperlessparts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: docs.paperlessparts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.paperlessparts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paperless Parts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paperless Parts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Paperless Parts
provider_slug: paperless-parts
slug: paperless-parts-domain-security
source_filename: paperless-parts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paperlessparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.paperlessparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.paperlessparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paperlessparts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/security/paperless-parts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Quoting
- CNC Machining
- Sheet Metal
- ERP
- CRM
- Job Shops
- Aerospace and Defense
- Pricing
- Estimating
- Industrial
---
