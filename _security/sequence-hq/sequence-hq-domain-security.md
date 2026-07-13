---
api_specs:
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Customers API
  slug: sequence-hq-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Usage & Metering API
  slug: sequence-hq-usage-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Billing Schedules API
  slug: sequence-hq-billing-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Invoices & Credit Notes API
  slug: sequence-hq-invoices-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Products & Prices API
  slug: sequence-hq-products-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Quotes API
  slug: sequence-hq-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sequencehq.com
  spf: true
hosts:
- cert_expires: Sep  4 20:59:52 2026 GMT
  host: sequencehq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: www.sequencehq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 16:18:39 2026 GMT
  host: eu.sequencehq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 14:56:23 2026 GMT
  host: docs.sequencehq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequence Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequence, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sequence
provider_slug: sequence-hq
slug: sequence-hq-domain-security
source_filename: sequence-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequencehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:59:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.sequencehq.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n- host: eu.sequencehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:18:39 2026 GMT\n  hsts: false\n- host: docs.sequencehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:56:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sequencehq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/security/sequence-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Billing
- Usage-Based Billing
- Revenue Recognition
- Metering
- Invoicing
- Pricing
- Revenue Orchestration
- FinOps
---
