---
api_specs:
- filename: paymate-businesses-api-openapi.yml
  format: yaml
  label: PayMate Businesses API
  slug: paymate-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-businesses-api-openapi.yml
- filename: paymate-cards-api-openapi.yml
  format: yaml
  label: PayMate Cards API
  slug: paymate-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-cards-api-openapi.yml
- filename: paymate-collections-api-openapi.yml
  format: yaml
  label: PayMate Collections API
  slug: paymate-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-collections-api-openapi.yml
- filename: paymate-contacts-api-openapi.yml
  format: yaml
  label: PayMate Contacts API
  slug: paymate-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-contacts-api-openapi.yml
- filename: paymate-payments-api-openapi.yml
  format: yaml
  label: PayMate Payments API
  slug: paymate-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-payments-api-openapi.yml
- filename: paymate-reference-api-openapi.yml
  format: yaml
  label: PayMate Reference API
  slug: paymate-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-reference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paymate.in
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paymate.my
  spf: true
hosts:
- cert_expires: Oct 22 10:43:55 2026 GMT
  host: paymate.in
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 27 10:20:26 2026 GMT
  host: api.paymate.my
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: uat.paymate.co.in
  https: false
kind: domain-security
layout: security
method: probed
name: Paymate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayMate, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PayMate
provider_slug: paymate
slug: paymate-domain-security
source_filename: paymate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paymate.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 10:43:55 2026 GMT\n  hsts: null\n- host: api.paymate.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 10:20:26 2026 GMT\n  hsts: null\n- host: uat.paymate.co.in\n  https: false\ndomains:\n- domain: paymate.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: paymate.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/security/paymate-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Payments
- B2B Payments
- Accounts Payable
- Accounts Receivable
- Supply Chain Finance
- Invoice Discounting
- Working Capital
- Commercial Cards
- Financial Services
- India
- Fintech
- Company
---
