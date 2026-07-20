---
api_specs:
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Banking API
  slug: prometeo-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Account Validation API
  slug: prometeo-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Cross-Border Payments API
  slug: prometeo-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Payment API
  slug: prometeo-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Identity API (CURP)
  slug: prometeo-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
description: ''
domains:
- domain: prometeoapi.com
  note: Primary brand domain. Production API surfaces are served from the prometeoapi.net apex; sandbox surfaces from *.sandbox.prometeoapi.com. DNSSEC / CAA / SPF / DMARC not reconciled in this artifact - verify on the next live-probe pass.
hosts:
- host: prometeoapi.com
  https: true
  note: Marketing and developer entry point; probe TLS on reconciliation.
- host: docs.prometeoapi.com
  https: true
  note: Developer documentation (ReadMe-hosted).
- host: banking.prometeoapi.net
  https: true
  note: Banking API production host.
- host: account-validation.prometeoapi.net
  https: true
  note: Account Validation API production host.
- host: crossborder.secure.prometeoapi.net
  https: true
  note: Cross-Border API production host (v1 base path).
- host: payment.prometeoapi.net
  https: true
  note: Payment API production host.
- host: identity.prometeoapi.net
  https: true
  note: Identity (CURP) API production host.
- host: fiscal.prometeoapi.net
  https: true
  note: Fiscal (DIAN / SAT / CEP / BCU) API production host.
kind: domain-security
layout: security
method: probed
name: Prometeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prometeo, probed live across 8 host(s) and 1 registrable domain(s). 8 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prometeo
provider_slug: prometeo
slug: prometeo-domain-security
source_filename: prometeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prometeoapi.com\n  https: true\n  note: Marketing and developer entry point; probe TLS on reconciliation.\n- host: docs.prometeoapi.com\n  https: true\n  note: Developer documentation (ReadMe-hosted).\n- host: banking.prometeoapi.net\n  https: true\n  note: Banking API production host.\n- host: account-validation.prometeoapi.net\n  https: true\n  note: Account Validation API production host.\n- host: crossborder.secure.prometeoapi.net\n  https: true\n  note: Cross-Border API production host (v1 base path).\n- host: payment.prometeoapi.net\n  https: true\n  note: Payment API production host.\n- host: identity.prometeoapi.net\n  https: true\n  note: Identity (CURP) API production host.\n- host: fiscal.prometeoapi.net\n  https: true\n  note: Fiscal (DIAN / SAT / CEP / BCU) API production host.\ndomains:\n- domain: prometeoapi.com\n  note: >-\n    Primary brand\
  \ domain. Production API surfaces are served from the\n    prometeoapi.net apex; sandbox surfaces from *.sandbox.prometeoapi.com.\n    DNSSEC / CAA / SPF / DMARC not reconciled in this artifact - verify on the\n    next live-probe pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/security/prometeo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Open Banking
- Payments
- FinTech
- LatAm
- Financial Data
- Account Validation
- Cross-Border
---
