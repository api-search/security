---
api_specs:
- filename: visa-acceptance-captures-api-openapi.yml
  format: yaml
  label: Visa Acceptance Captures API
  slug: visa-acceptance-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-captures-api-openapi.yml
- filename: visa-acceptance-invoices-api-openapi.yml
  format: yaml
  label: Visa Acceptance Invoices API
  slug: visa-acceptance-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-invoices-api-openapi.yml
- filename: visa-acceptance-pay-by-link-api-openapi.yml
  format: yaml
  label: Visa Acceptance Pay by Link API
  slug: visa-acceptance-pay-by-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-pay-by-link-api-openapi.yml
- filename: visa-acceptance-payments-api-openapi.yml
  format: yaml
  label: Visa Acceptance Payments API
  slug: visa-acceptance-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-payments-api-openapi.yml
- filename: visa-acceptance-refunds-api-openapi.yml
  format: yaml
  label: Visa Acceptance Refunds API
  slug: visa-acceptance-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-refunds-api-openapi.yml
- filename: visa-acceptance-voids-api-openapi.yml
  format: yaml
  label: Visa Acceptance Voids API
  slug: visa-acceptance-voids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-voids-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@visa.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: visaacceptance.com
  spf: true
hosts:
- cert_expires: Oct 19 04:32:38 2026 GMT
  host: developer.visaacceptance.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.visaacceptance.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: apitest.visaacceptance.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Visa Acceptance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visa Acceptance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Visa Acceptance
provider_slug: visa-acceptance
slug: visa-acceptance-domain-security
source_filename: visa-acceptance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.visaacceptance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 04:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.visaacceptance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\n- host: apitest.visaacceptance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: visaacceptance.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hostmaster@visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/security/visa-acceptance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- E-Commerce
- Fintech
- Credit Cards
- Invoicing
- Payment Links
- Digital Wallets
---
