---
api_specs:
- filename: paytronix-check-api-openapi.yml
  format: yaml
  label: Paytronix Check API
  slug: paytronix-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-check-api-openapi.yml
- filename: paytronix-enrollment-api-openapi.yml
  format: yaml
  label: Paytronix Enrollment API
  slug: paytronix-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-enrollment-api-openapi.yml
- filename: paytronix-gift-api-openapi.yml
  format: yaml
  label: Paytronix Gift API
  slug: paytronix-gift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-gift-api-openapi.yml
- filename: paytronix-guest-api-openapi.yml
  format: yaml
  label: Paytronix Guest API
  slug: paytronix-guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-guest-api-openapi.yml
- filename: paytronix-menu-items-api-openapi.yml
  format: yaml
  label: Paytronix Menu Items API
  slug: paytronix-menu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-menu-items-api-openapi.yml
- filename: paytronix-oauth-api-openapi.yml
  format: yaml
  label: Paytronix OAuth API
  slug: paytronix-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-oauth-api-openapi.yml
- filename: paytronix-orders-api-openapi.yml
  format: yaml
  label: Paytronix Orders API
  slug: paytronix-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-orders-api-openapi.yml
- filename: paytronix-payment-api-openapi.yml
  format: yaml
  label: Paytronix Payment API
  slug: paytronix-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-payment-api-openapi.yml
- filename: paytronix-restaurants-api-openapi.yml
  format: yaml
  label: Paytronix Restaurants API
  slug: paytronix-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-restaurants-api-openapi.yml
- filename: paytronix-search-api-openapi.yml
  format: yaml
  label: Paytronix Search API
  slug: paytronix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-search-api-openapi.yml
- filename: paytronix-store-api-openapi.yml
  format: yaml
  label: Paytronix Store API
  slug: paytronix-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-store-api-openapi.yml
- filename: paytronix-transaction-api-openapi.yml
  format: yaml
  label: Paytronix Transaction API
  slug: paytronix-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paytronix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opendining.net
  spf: true
hosts:
- cert_expires: Oct  1 17:56:53 2026 GMT
  host: www.paytronix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:31:33 2026 GMT
  host: developers.paytronix.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: docs.opendining.net
  https: false
kind: domain-security
layout: security
method: probed
name: Paytronix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paytronix, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paytronix
provider_slug: paytronix
slug: paytronix-domain-security
source_filename: paytronix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paytronix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:56:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.paytronix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 19:31:33 2026 GMT\n  hsts: false\n- host: docs.opendining.net\n  https: false\ndomains:\n- domain: paytronix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opendining.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/security/paytronix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Loyalty
- Gift Cards
- Online Ordering
- Guest Engagement
- Payments
- Messaging
---
