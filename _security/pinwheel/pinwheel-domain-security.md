---
api_specs:
- filename: pinwheel-accounts-api-openapi.yml
  format: yaml
  label: Pinwheel Accounts API
  slug: pinwheel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-accounts-api-openapi.yml
- filename: pinwheel-api-keys-api-openapi.yml
  format: yaml
  label: Pinwheel API Keys API
  slug: pinwheel-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-api-keys-api-openapi.yml
- filename: pinwheel-company-connect-api-openapi.yml
  format: yaml
  label: Pinwheel Company Connect API
  slug: pinwheel-company-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-company-connect-api-openapi.yml
- filename: pinwheel-direct-deposit-allocations-api-openapi.yml
  format: yaml
  label: Pinwheel Direct Deposit Allocations API
  slug: pinwheel-direct-deposit-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-direct-deposit-allocations-api-openapi.yml
- filename: pinwheel-earnings-stream-api-openapi.yml
  format: yaml
  label: Pinwheel Earnings Stream API
  slug: pinwheel-earnings-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-earnings-stream-api-openapi.yml
- filename: pinwheel-employers-and-platforms-api-openapi.yml
  format: yaml
  label: Pinwheel Employers and Platforms API
  slug: pinwheel-employers-and-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-employers-and-platforms-api-openapi.yml
- filename: pinwheel-end-users-api-openapi.yml
  format: yaml
  label: Pinwheel End Users API
  slug: pinwheel-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-end-users-api-openapi.yml
- filename: pinwheel-income-and-employment-api-openapi.yml
  format: yaml
  label: Pinwheel Income and Employment API
  slug: pinwheel-income-and-employment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-income-and-employment-api-openapi.yml
- filename: pinwheel-jobs-api-openapi.yml
  format: yaml
  label: Pinwheel Jobs API
  slug: pinwheel-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-jobs-api-openapi.yml
- filename: pinwheel-link-tokens-api-openapi.yml
  format: yaml
  label: Pinwheel Link Tokens API
  slug: pinwheel-link-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-link-tokens-api-openapi.yml
- filename: pinwheel-sandbox-api-openapi.yml
  format: yaml
  label: Pinwheel Sandbox API
  slug: pinwheel-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-sandbox-api-openapi.yml
- filename: pinwheel-tax-forms-api-openapi.yml
  format: yaml
  label: Pinwheel Tax Forms API
  slug: pinwheel-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-tax-forms-api-openapi.yml
- filename: pinwheel-verification-reports-api-openapi.yml
  format: yaml
  label: Pinwheel Verification Reports API
  slug: pinwheel-verification-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-verification-reports-api-openapi.yml
- filename: pinwheel-webhooks-api-openapi.yml
  format: yaml
  label: Pinwheel Webhooks API
  slug: pinwheel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pinwheelapi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpinwheel.com
  spf: true
hosts:
- cert_expires: Sep 28 11:56:32 2026 GMT
  host: www.pinwheelapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.getpinwheel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: sandbox.getpinwheel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinwheel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinwheel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pinwheel
provider_slug: pinwheel
slug: pinwheel-domain-security
source_filename: pinwheel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinwheelapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:56:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getpinwheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox.getpinwheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pinwheelapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getpinwheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/security/pinwheel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payroll
- Direct Deposit
- Income Verification
- Employment
- Tax Forms
- Fintech
- Open Finance
- Bill Switching
- Financial Data
---
