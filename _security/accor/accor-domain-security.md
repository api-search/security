---
api_specs:
- filename: accor-businessoffers-api-openapi.yml
  format: yaml
  label: Accor Businessoffers API
  slug: accor-businessoffers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-businessoffers-api-openapi.yml
- filename: accor-catalog-api-openapi.yml
  format: yaml
  label: Accor Catalog API
  slug: accor-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-catalog-api-openapi.yml
- filename: accor-contracts-api-openapi.yml
  format: yaml
  label: Accor Contracts API
  slug: accor-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-contracts-api-openapi.yml
- filename: accor-customer-api-openapi.yml
  format: yaml
  label: Accor Customer API
  slug: accor-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-customer-api-openapi.yml
- filename: accor-hotel-interface-api-openapi.yml
  format: yaml
  label: Accor Hotel Interface API
  slug: accor-hotel-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-hotel-interface-api-openapi.yml
- filename: accor-loyalty-api-openapi.yml
  format: yaml
  label: Accor Loyalty API
  slug: accor-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-loyalty-api-openapi.yml
- filename: accor-payment-api-openapi.yml
  format: yaml
  label: Accor Payment API
  slug: accor-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-payment-api-openapi.yml
- filename: accor-private-publication-check-api-openapi.yml
  format: yaml
  label: Accor Private Publication Check API
  slug: accor-private-publication-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-private-publication-check-api-openapi.yml
- filename: accor-referentials-api-openapi.yml
  format: yaml
  label: Accor Referentials API
  slug: accor-referentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-referentials-api-openapi.yml
- filename: accor-secure-api-openapi.yml
  format: yaml
  label: Accor Secure API
  slug: accor-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-secure-api-openapi.yml
- filename: accor-test-travel-concierge-new-api-openapi.yml
  format: yaml
  label: Accor Test Travel Concierge New API
  slug: accor-test-travel-concierge-new-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-test-travel-concierge-new-api-openapi.yml
- filename: accor-wallet-api-openapi.yml
  format: yaml
  label: Accor Wallet API
  slug: accor-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-wallet-api-openapi.yml
- filename: accor-health-check-api-openapi.yml
  format: yaml
  label: Accor Health Check API
  slug: accor-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/accor-health-check-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: accor.com
  spf: true
hosts:
- cert_expires: Nov 25 07:33:13 2026 GMT
  host: accor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Accor
provider_slug: accor
slug: accor-domain-security
source_filename: accor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 07:33:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: accor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/security/accor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Travel
- Hotels
- Technology
---
