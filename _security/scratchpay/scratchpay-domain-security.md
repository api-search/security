---
api_specs:
- filename: scratchpay-scratchpay-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Borrower Application API
  slug: scratchpay-borrower-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml
- filename: scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Care Credit API
  slug: scratchpay-care-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
- filename: scratchpay-partner-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Partner Result API
  slug: scratchpay-partner-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-partner-1.0.0-apis-swagger.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scratchpay.com
  spf: true
hosts:
- cert_expires: Sep 23 14:47:53 2026 GMT
  host: scratchpay.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scratchpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scratchpay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scratchpay
provider_slug: scratchpay
slug: scratchpay-domain-security
source_filename: scratchpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scratchpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:47:53 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: scratchpay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/security/scratchpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financing
- Payments
- Lending
- Veterinary
- Healthcare
- Fintech
- Buy Now Pay Later
- Point of Sale
---
