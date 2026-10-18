---
api_specs:
- filename: apiposture-account-api-openapi.yml
  format: yaml
  label: APIPosture Account API
  slug: apiposture-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-account-api-openapi.yml
- filename: apiposture-admin-api-openapi.yml
  format: yaml
  label: APIPosture Admin API
  slug: apiposture-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-admin-api-openapi.yml
- filename: apiposture-apiposture-api-openapi.yml
  format: yaml
  label: APIPosture Apiposture API
  slug: apiposture-apiposture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-apiposture-api-openapi.yml
- filename: apiposture-blagoculjak-api-openapi.yml
  format: yaml
  label: APIPosture Blagoculjak API
  slug: apiposture-blagoculjak-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-blagoculjak-api-openapi.yml
- filename: apiposture-cart-api-openapi.yml
  format: yaml
  label: APIPosture Cart API
  slug: apiposture-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-cart-api-openapi.yml
- filename: apiposture-finalize-order-api-openapi.yml
  format: yaml
  label: APIPosture Finalize Order API
  slug: apiposture-finalize-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-finalize-order-api-openapi.yml
- filename: apiposture-install-api-openapi.yml
  format: yaml
  label: APIPosture Install API
  slug: apiposture-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-install-api-openapi.yml
- filename: apiposture-installer-api-openapi.yml
  format: yaml
  label: APIPosture Installer API
  slug: apiposture-installer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-installer-api-openapi.yml
- filename: apiposture-merchant-api-openapi.yml
  format: yaml
  label: APIPosture Merchant API
  slug: apiposture-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-merchant-api-openapi.yml
- filename: apiposture-payment-intent-api-openapi.yml
  format: yaml
  label: APIPosture Payment Intent API
  slug: apiposture-payment-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-payment-intent-api-openapi.yml
- filename: apiposture-resources-api-openapi.yml
  format: yaml
  label: APIPosture Resources API
  slug: apiposture-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-resources-api-openapi.yml
- filename: apiposture-status-api-openapi.yml
  format: yaml
  label: APIPosture Status API
  slug: apiposture-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-status-api-openapi.yml
- filename: apiposture-transactions-api-openapi.yml
  format: yaml
  label: APIPosture Transactions API
  slug: apiposture-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-transactions-api-openapi.yml
- filename: apiposture-users-api-openapi.yml
  format: yaml
  label: APIPosture Users API
  slug: apiposture-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/openapi/apiposture-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiposture.com
  spf: true
hosts:
- cert_expires: Dec 10 14:26:55 2026 GMT
  host: apiposture.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apiposture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIPosture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: APIPosture
provider_slug: apiposture
slug: apiposture-domain-security
source_filename: apiposture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiposture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 14:26:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: apiposture.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiposture/refs/heads/main/security/apiposture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Security
- Compliance
- Automation
- DevOps
- Monitoring
---
