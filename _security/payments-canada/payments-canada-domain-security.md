---
api_specs:
- filename: rtr-inbound-participant-payment-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Participant Payment API
  slug: rtr-inbound-participant-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-participant-payment-api-openapi.yml
- filename: rtr-inbound-csp-heartbeat-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Exchange Heartbeat API
  slug: rtr-inbound-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-csp-heartbeat-api-openapi.yml
- filename: rtr-interest-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Interest Report API
  slug: rtr-interest-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-interest-report-api-openapi.yml
- filename: rtr-balance-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Payment Capacity Balance Report API
  slug: rtr-balance-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-balance-report-api-openapi.yml
- filename: fif-extracts-api-openapi.yml
  format: yaml
  label: FIF Extracts API
  slug: fif-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-extracts-api-openapi.yml
- filename: fif-branch-api-openapi.yml
  format: yaml
  label: FIF Branch API
  slug: fif-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-branch-api-openapi.yml
- filename: ccin-extracts-api-openapi.yml
  format: yaml
  label: CCIN Extracts API
  slug: ccin-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-extracts-api-openapi.yml
- filename: ccin-lookup-api-openapi.yml
  format: yaml
  label: CCIN Lookup API
  slug: ccin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-lookup-api-openapi.yml
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
