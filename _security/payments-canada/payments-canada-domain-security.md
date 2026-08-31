---
api_specs:
- filename: payments-canada-application-level-heartbeat-api-openapi.yml
  format: yaml
  label: Payments Canada application level heartbeat API
  slug: payments-canada-application-level-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-application-level-heartbeat-api-openapi.yml
- filename: payments-canada-ccin-extract-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Ccin Extract Resource API
  slug: payments-canada-ccin-extract-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-ccin-extract-resource-api-openapi.yml
- filename: payments-canada-fif-branches-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Fif Branches Resource API
  slug: payments-canada-fif-branches-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-fif-branches-resource-api-openapi.yml
- filename: payments-canada-fif-extracts-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Fif Extracts Resource API
  slug: payments-canada-fif-extracts-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-fif-extracts-resource-api-openapi.yml
- filename: payments-canada-interest-report-api-openapi.yml
  format: yaml
  label: Payments Canada Interest Report API
  slug: payments-canada-interest-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-interest-report-api-openapi.yml
- filename: payments-canada-master-extract-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Master Extract Resource API
  slug: payments-canada-master-extract-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-master-extract-resource-api-openapi.yml
- filename: payments-canada-report-api-openapi.yml
  format: yaml
  label: Payments Canada Report API
  slug: payments-canada-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-report-api-openapi.yml
- filename: payments-canada-single-credit-transfer-api-openapi.yml
  format: yaml
  label: Payments Canada single credit transfer API
  slug: payments-canada-single-credit-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-single-credit-transfer-api-openapi.yml
- filename: payments-canada-single-credit-transfer-status-enquiry-api-openapi.yml
  format: yaml
  label: Payments Canada single credit transfer status enquiry API
  slug: payments-canada-single-credit-transfer-status-enquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-single-credit-transfer-status-enquiry-api-openapi.yml
- filename: payments-canada-update-extract-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Update Extract Resource API
  slug: payments-canada-update-extract-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-update-extract-resource-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payments.ca
  spf: true
hosts:
- cert_expires: Sep  9 14:48:05 2026 GMT
  host: www.payments.ca
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: developer.payments.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.payments.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payments Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payments Canada, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Payments Canada
provider_slug: payments-canada
slug: payments-canada-domain-security
source_filename: payments-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payments.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.payments.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.payments.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: payments.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/security/payments-canada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Payments
- Canada
- Payment Infrastructure
- Clearing and Settlement
- Real-Time Rail
- ISO 20022
- Lynx
- Crown Corporation
- Faster Payments
---
