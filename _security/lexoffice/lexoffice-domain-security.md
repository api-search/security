---
api_specs:
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Contacts API
  slug: lexoffice-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Invoices API
  slug: lexoffice-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Quotations API
  slug: lexoffice-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Order Confirmations API
  slug: lexoffice-order-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Delivery Notes API
  slug: lexoffice-delivery-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Credit Notes API
  slug: lexoffice-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Dunnings API
  slug: lexoffice-dunnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Vouchers API
  slug: lexoffice-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Event Subscriptions API
  slug: lexoffice-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Payments API
  slug: lexoffice-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Profile and Metadata API
  slug: lexoffice-profile-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lexware.de
  spf: true
  spf_policy: -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lexware.io
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.lexware.io
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: developers.lexware.io
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.lexware.de
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: app.lexware.de
  hsts: true
  hsts_max_age: 63072000
  http_status: 301
  https: true
kind: domain-security
layout: security
method: probed
name: Lexoffice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lexoffice, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: lexoffice
provider_slug: lexoffice
slug: lexoffice-domain-security
source_filename: lexoffice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.lexware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\n  http_status: 200\n- host: developers.lexware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n  http_status: 200\n- host: www.lexware.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n  http_status: 200\n- host: app.lexware.de\n  https: true\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  http_status: 301\ndomains:\n- domain: lexware.de\n  dnssec: true\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lexware.io\n  dnssec: false\n  caa: []\n  dmarc: true\n  dmarc_policy: reject\nnotes: >-\n  The current API gateway (api.lexware.io) and developer portal\n  (developers.lexware.io)\
  \ serve valid TLSv1.3 certificates but did not return an\n  HSTS header on the probed root responses; the customer web app (app.lexware.de)\n  does send HSTS (max-age 63072000, includeSubDomains). The primary corporate\n  domain lexware.de is DNSSEC-signed with an SPF hard-fail (-all) and a DMARC\n  quarantine policy; the lexware.io API domain publishes a strict DMARC reject\n  policy. No CAA records were observed on either apex domain at probe time. The\n  legacy lexoffice.io API host was retired at the end of 2025 and was not probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/security/lexoffice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Invoicing
- Bookkeeping
- Finance
- Germany
- Vouchers
- Contacts
- SaaS
- Financial Software
---
