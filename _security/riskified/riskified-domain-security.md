---
api_specs:
- filename: riskified-automation-endpoints-api-openapi.yml
  format: yaml
  label: Riskified Automation Endpoints API
  slug: riskified-automation-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-automation-endpoints-api-openapi.yml
- filename: riskified-customer-actions-api-openapi.yml
  format: yaml
  label: Riskified Customer Actions API
  slug: riskified-customer-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-customer-actions-api-openapi.yml
- filename: riskified-customer-management-api-openapi.yml
  format: yaml
  label: Riskified Customer Management API
  slug: riskified-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-customer-management-api-openapi.yml
- filename: riskified-order-pre-auth-review-and-psd2-3ds-cvv-recommendations-api-openapi.yml
  format: yaml
  label: Riskified Order Pre-Auth Review and PSD2/3DS/CVV Recommendations API
  slug: riskified-order-pre-auth-review-and-psd2-3ds-cvv-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-order-pre-auth-review-and-psd2-3ds-cvv-recommendations-api-openapi.yml
- filename: riskified-otp-recover-sync-flow-api-openapi.yml
  format: yaml
  label: Riskified OTP Recover (Sync flow) API
  slug: riskified-otp-recover-sync-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-otp-recover-sync-flow-api-openapi.yml
- filename: riskified-post-authorization-flow-api-openapi.yml
  format: yaml
  label: Riskified Post-Authorization Flow API
  slug: riskified-post-authorization-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-post-authorization-flow-api-openapi.yml
- filename: riskified-pre-authorization-flow-api-openapi.yml
  format: yaml
  label: Riskified Pre-Authorization Flow API
  slug: riskified-pre-authorization-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-pre-authorization-flow-api-openapi.yml
- filename: riskified-refunds-api-openapi.yml
  format: yaml
  label: Riskified Refunds API
  slug: riskified-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-refunds-api-openapi.yml
- filename: riskified-returns-api-openapi.yml
  format: yaml
  label: Riskified Returns API
  slug: riskified-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-returns-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: riskified.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.riskified.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:40:19 2026 GMT
  host: developers.riskified.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: wh.riskified.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Riskified Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riskified, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Riskified
provider_slug: riskified
slug: riskified-domain-security
source_filename: riskified-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riskified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n- host: developers.riskified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:40:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wh.riskified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: riskified.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/security/riskified-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Chargebacks
- E-Commerce
- Payments
- Risk Management
- Machine Learning
- Account Takeover
- Policy Abuse
- 3D
- PSD2
- Returns
---
