---
api_specs:
- filename: credilinqai-authentication-api-openapi.yml
  format: yaml
  label: Credilinq.ai Authentication API
  slug: credilinqai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-authentication-api-openapi.yml
- filename: credilinqai-customers-api-openapi.yml
  format: yaml
  label: Credilinq.ai Customers API
  slug: credilinqai-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-customers-api-openapi.yml
- filename: credilinqai-kyc-api-openapi.yml
  format: yaml
  label: Credilinq.ai KYC API
  slug: credilinqai-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-kyc-api-openapi.yml
- filename: credilinqai-loans-api-openapi.yml
  format: yaml
  label: Credilinq.ai Loans API
  slug: credilinqai-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-loans-api-openapi.yml
- filename: credilinqai-miscellaneous-api-openapi.yml
  format: yaml
  label: Credilinq.ai Miscellaneous API
  slug: credilinqai-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-miscellaneous-api-openapi.yml
- filename: credilinqai-onboarding-api-openapi.yml
  format: yaml
  label: Credilinq.ai Onboarding API
  slug: credilinqai-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-onboarding-api-openapi.yml
- filename: credilinqai-payment-api-openapi.yml
  format: yaml
  label: Credilinq.ai Payment API
  slug: credilinqai-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-payment-api-openapi.yml
- filename: credilinqai-report-api-openapi.yml
  format: yaml
  label: Credilinq.ai Report API
  slug: credilinqai-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-report-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: credilinq.ai
  spf: true
hosts:
- cert_expires: Sep 16 04:00:24 2026 GMT
  host: credilinq.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: sandbox-api.credilinq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: stage-api.credilinq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Credilinqai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credilinq.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credilinq.ai
provider_slug: credilinqai
slug: credilinqai-domain-security
source_filename: credilinqai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: credilinq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:00:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox-api.credilinq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: stage-api.credilinq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: credilinq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/security/credilinqai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- BNPL
- Credit
- Payments
- KYC
- B2B
---
