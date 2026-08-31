---
api_specs:
- filename: insforge-admin-api-openapi.yml
  format: yaml
  label: Insforge Admin API
  slug: insforge-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-admin-api-openapi.yml
- filename: insforge-channels-api-openapi.yml
  format: yaml
  label: Insforge Channels API
  slug: insforge-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-channels-api-openapi.yml
- filename: insforge-client-api-openapi.yml
  format: yaml
  label: Insforge Client API
  slug: insforge-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-client-api-openapi.yml
- filename: insforge-configuration-api-openapi.yml
  format: yaml
  label: Insforge Configuration API
  slug: insforge-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-configuration-api-openapi.yml
- filename: insforge-messages-api-openapi.yml
  format: yaml
  label: Insforge Messages API
  slug: insforge-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-messages-api-openapi.yml
- filename: insforge-payment-webhooks-api-openapi.yml
  format: yaml
  label: Insforge Payment Webhooks API
  slug: insforge-payment-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-payment-webhooks-api-openapi.yml
- filename: insforge-permissions-api-openapi.yml
  format: yaml
  label: Insforge Permissions API
  slug: insforge-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-permissions-api-openapi.yml
- filename: insforge-razorpay-payments-api-openapi.yml
  format: yaml
  label: Insforge Razorpay Payments API
  slug: insforge-razorpay-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-razorpay-payments-api-openapi.yml
- filename: insforge-s3-access-keys-api-openapi.yml
  format: yaml
  label: Insforge S3 Access Keys API
  slug: insforge-s3-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-s3-access-keys-api-openapi.yml
- filename: insforge-s3-protocol-api-openapi.yml
  format: yaml
  label: Insforge S3 Protocol API
  slug: insforge-s3-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-s3-protocol-api-openapi.yml
- filename: insforge-stripe-payments-api-openapi.yml
  format: yaml
  label: Insforge Stripe Payments API
  slug: insforge-stripe-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-stripe-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insforge.dev
  spf: true
hosts:
- cert_expires: Sep  7 21:24:55 2026 GMT
  host: insforge.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:28:21 2026 GMT
  host: docs.insforge.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.insforge.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insforge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Insforge
provider_slug: insforge
slug: insforge-domain-security
source_filename: insforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:24:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.insforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.insforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: insforge.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/security/insforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backend as a Service
- Agent Native
- Cloud Infrastructure
- Database
- Authentication
- Storage
- Serverless
- Edge Functions
- AI Gateway
- Payments
- Real-Time
- Open-Source
- Y Combinator
---
