---
api_specs:
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Hosted Payment Page API
  slug: paytabs-hosted-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Managed Form API
  slug: paytabs-managed-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Own Form API
  slug: paytabs-own-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Transaction Management API
  slug: paytabs-transaction-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Token & Recurring Billing API
  slug: paytabs-token-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Invoices API
  slug: paytabs-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
description: ''
domains: []
hosts:
- host: paytabs.com
  http_status: 200
  https: true
- host: secure.paytabs.com
  http_status: 301
  https: true
  region: UAE / default
- host: secure.paytabs.sa
  http_status: 301
  https: true
  region: Saudi Arabia (KSA)
- host: secure-egypt.paytabs.com
  http_status: 301
  https: true
  region: Egypt
- host: docs.paytabs.com
  https: true
  region: Technical portal
kind: domain-security
layout: security
method: probed
name: Paytabs Domain Security
name_suffix: Domain Security
overview: Domain security posture for PayTabs, probed live across 5 host(s) and 0 registrable domain(s). 5 host(s) serve HTTPS; 0 advertise HSTS.
provider_name: PayTabs
provider_slug: paytabs
slug: paytabs-domain-security
source_filename: paytabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live HTTP probes of apis.yml + OpenAPI region hosts\nnotes: >-\n  PayTabs serves the PT2 REST API on region-specific hosts. The `secure*` hosts\n  redirect (301) plain GETs but terminate TLS and serve the documented POST\n  endpoints. Using the wrong region host for a given profile/key causes\n  authentication (401) errors per PayTabs documentation.\nhosts:\n- host: paytabs.com\n  https: true\n  http_status: 200\n- host: secure.paytabs.com\n  https: true\n  http_status: 301\n  region: UAE / default\n- host: secure.paytabs.sa\n  https: true\n  http_status: 301\n  region: Saudi Arabia (KSA)\n- host: secure-egypt.paytabs.com\n  https: true\n  http_status: 301\n  region: Egypt\n- host: docs.paytabs.com\n  https: true\n  region: Technical portal\nregion_hosts:\n- secure.paytabs.com\n- secure.paytabs.sa\n- secure-egypt.paytabs.com\n- secure-oman.paytabs.com\n- secure-jordan.paytabs.com\n- secure-kuwait.paytabs.com\n- secure-iraq.paytabs.com\n\
  - secure-morocco.paytabs.com\n- secure-doha.paytabs.com\n- secure-global.paytabs.com\ntransport_security:\n  tls: true\n  pci_dss: PCI DSS Level 1 (card processing)\n  three_d_secure: EMV 3-D Secure 2 (via Modirum), first deployment in KSA\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/security/paytabs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- Saudi Arabia
- Cards
- mada
---
