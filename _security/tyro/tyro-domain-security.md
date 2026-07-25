---
api_specs:
- filename: tyro-connect-pay.yml
  format: yaml
  label: Tyro Connect Pay API
  slug: tyro-connect-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-pay.yml
- filename: tyro-pos-pay-terminal.yml
  format: yaml
  label: Tyro Pay Terminal API
  slug: tyro-pos-pay-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-pos-pay-terminal.yml
- filename: tyro-pos-embedded-payments.yml
  format: yaml
  label: Tyro Embedded Payments API
  slug: tyro-pos-embedded-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-pos-embedded-payments.yml
- filename: tyro-connect-booking.yml
  format: yaml
  label: Tyro Connect Booking API
  slug: tyro-connect-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-booking.yml
- filename: tyro-connect-ordering.yml
  format: yaml
  label: Tyro Connect Ordering API
  slug: tyro-connect-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-ordering.yml
- filename: tyro-connect-menu.yml
  format: yaml
  label: Tyro Connect Menu API
  slug: tyro-connect-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-menu.yml
- filename: tyro-connect-tables.yml
  format: yaml
  label: Tyro Connect Tables Management API
  slug: tyro-connect-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-tables.yml
- filename: tyro-connect-sales.yml
  format: yaml
  label: Tyro Connect Sales Data API
  slug: tyro-connect-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-sales.yml
- filename: tyro-connect-reporting.yml
  format: yaml
  label: Tyro Connect Reporting API
  slug: tyro-connect-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-reporting.yml
- filename: tyro-connect-loyalty.yml
  format: yaml
  label: Tyro Connect Loyalty Data API
  slug: tyro-connect-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-loyalty.yml
- filename: tyro-connect-refunds.yml
  format: yaml
  label: Tyro Connect Refunds API
  slug: tyro-connect-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-refunds.yml
- filename: tyro-connect-locations.yml
  format: yaml
  label: Tyro Connect Location API
  slug: tyro-connect-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-locations.yml
- filename: tyro-connect-referrals.yml
  format: yaml
  label: Tyro Connect Referrals API
  slug: tyro-connect-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-referrals.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tyro.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.tyro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 08:22:26 2026 GMT
  host: docs.connect.tyro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.tyro.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tyro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tyro Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tyro Payments
provider_slug: tyro
slug: tyro-domain-security
source_filename: tyro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tyro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: docs.connect.tyro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:22:26 2026 GMT\n  hsts: false\n- host: api.tyro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tyro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/security/tyro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Australia
- Merchant Acquiring
- Payment Gateway
- In-Person Payments
- EFTPOS
- Point of Sale
- Online Payments
- Tap to Pay
---
