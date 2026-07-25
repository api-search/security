---
api_specs:
- filename: przelewy24-additional-api-functionality-api-openapi.yml
  format: yaml
  label: Przelewy24 Additional API functionality API
  slug: przelewy24-additional-api-functionality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-additional-api-functionality-api-openapi.yml
- filename: przelewy24-additional-services-mass-payments-transactions-api-openapi.yml
  format: yaml
  label: Przelewy24 Additional services Mass Payments Transactions API
  slug: przelewy24-additional-services-mass-payments-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-additional-services-mass-payments-transactions-api-openapi.yml
- filename: przelewy24-apay-api-api-openapi.yml
  format: yaml
  label: Przelewy24 APay API API
  slug: przelewy24-apay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-apay-api-api-openapi.yml
- filename: przelewy24-blik-api-api-openapi.yml
  format: yaml
  label: Przelewy24 BLIK API API
  slug: przelewy24-blik-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-blik-api-api-openapi.yml
- filename: przelewy24-card-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Card API API
  slug: przelewy24-card-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-card-api-api-openapi.yml
- filename: przelewy24-ekspres-p24-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Ekspres P24 API API
  slug: przelewy24-ekspres-p24-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-ekspres-p24-api-api-openapi.yml
- filename: przelewy24-gpay-api-api-openapi.yml
  format: yaml
  label: Przelewy24 GPay API API
  slug: przelewy24-gpay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-gpay-api-api-openapi.yml
- filename: przelewy24-marketplace-management-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Marketplace Management API API
  slug: przelewy24-marketplace-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-marketplace-management-api-api-openapi.yml
- filename: przelewy24-marketplace-merchant-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Marketplace Merchant API API
  slug: przelewy24-marketplace-merchant-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-marketplace-merchant-api-api-openapi.yml
- filename: przelewy24-marketplace-partner-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Marketplace Partner API API
  slug: przelewy24-marketplace-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-marketplace-partner-api-api-openapi.yml
- filename: przelewy24-recursion-dopayment-api-openapi.yml
  format: yaml
  label: Przelewy24 Recursion (doPayment) API
  slug: przelewy24-recursion-dopayment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-recursion-dopayment-api-openapi.yml
- filename: przelewy24-report-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Report API API
  slug: przelewy24-report-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-report-api-api-openapi.yml
- filename: przelewy24-transaction-service-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Transaction service API API
  slug: przelewy24-transaction-service-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-transaction-service-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: przelewy24.pl
  spf: true
hosts:
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: www.przelewy24.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: developers.przelewy24.pl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: secure.przelewy24.pl
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Przelewy24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Przelewy24, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Przelewy24
provider_slug: przelewy24
slug: przelewy24-domain-security
source_filename: przelewy24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.przelewy24.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.przelewy24.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.przelewy24.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: przelewy24.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/security/przelewy24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Bank Transfer
- BLIK
- Card Payments
- E-Commerce
- Poland
- Polish
- Multi-Currency
- Fintech
---
