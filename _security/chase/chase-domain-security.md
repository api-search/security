---
api_specs:
- filename: chase-account-and-customer-information-api-openapi.yml
  format: yaml
  label: Chase Account and Customer Information API
  slug: account-and-customer-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-account-and-customer-information-api-openapi.yml
- filename: chase-account-aggregation-user-consent-api-openapi.yml
  format: yaml
  label: Chase Account Aggregation User Consent API
  slug: account-aggregation-user-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-account-aggregation-user-consent-api-openapi.yml
- filename: chase-rewards-balance-api-openapi.yml
  format: yaml
  label: Chase Rewards Balance API
  slug: rewards-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-rewards-balance-api-openapi.yml
- filename: chase-loyalty-pay-with-points-order-service-api-openapi.yml
  format: yaml
  label: Chase Loyalty Pay with Points Order Service API
  slug: loyalty-pay-with-points-order-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml
- filename: chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml
  format: yaml
  label: Chase Loyalty Pay with Points Enrollment Service API
  slug: loyalty-pay-with-points-enrollment-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml
- filename: chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml
  format: yaml
  label: Chase Loyalty PCI Merchant Relationship Manager API
  slug: loyalty-pci-merchant-relationship-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chase.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.chase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: developer.chase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.chase.com
  https: false
kind: domain-security
layout: security
method: probed
name: Chase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chase, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chase
provider_slug: chase
slug: chase-domain-security
source_filename: chase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.chase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\n- host: api.chase.com\n  https: false\ndomains:\n- domain: chase.com\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/security/chase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Account Aggregation
- Banking
- Consent
- Credit Cards
- FDX
- Financial Services
- Loyalty
- Open Banking
- Pay with Points
- Rewards
---
