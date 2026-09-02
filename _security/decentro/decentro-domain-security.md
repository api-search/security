---
api_specs:
- filename: decentro-kyc-api-openapi.yml
  format: yaml
  label: Decentro KYC & Onboarding API
  slug: kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-kyc-api-openapi.yml
- filename: decentro-virtual-accounts-api-openapi.yml
  format: yaml
  label: Decentro Virtual Accounts API
  slug: virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-virtual-accounts-api-openapi.yml
- filename: decentro-accounts-api-openapi.yml
  format: yaml
  label: Decentro Accounts API
  slug: decentro-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-accounts-api-openapi.yml
- filename: decentro-collections-api-openapi.yml
  format: yaml
  label: Decentro Collections API
  slug: decentro-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-collections-api-openapi.yml
- filename: decentro-forensics-api-openapi.yml
  format: yaml
  label: Decentro Forensics API
  slug: decentro-forensics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-forensics-api-openapi.yml
- filename: decentro-journals-api-openapi.yml
  format: yaml
  label: Decentro Journals API
  slug: decentro-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-journals-api-openapi.yml
- filename: decentro-mandates-api-openapi.yml
  format: yaml
  label: Decentro Mandates API
  slug: decentro-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-mandates-api-openapi.yml
- filename: decentro-payouts-api-openapi.yml
  format: yaml
  label: Decentro Payouts API
  slug: decentro-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-payouts-api-openapi.yml
- filename: decentro-settlements-api-openapi.yml
  format: yaml
  label: Decentro Settlements API
  slug: decentro-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-settlements-api-openapi.yml
- filename: decentro-transactions-api-openapi.yml
  format: yaml
  label: Decentro Transactions API
  slug: decentro-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-transactions-api-openapi.yml
- filename: decentro-verification-api-openapi.yml
  format: yaml
  label: Decentro Verification API
  slug: decentro-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: decentro.tech
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: decentro.tech
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 01:20:13 2026 GMT
  host: docs.decentro.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: in.decentro.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decentro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decentro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Decentro
provider_slug: decentro
slug: decentro-domain-security
source_filename: decentro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decentro.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: docs.decentro.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:20:13 2026 GMT\n  hsts: null\n- host: in.decentro.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: decentro.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/security/decentro-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- Banking as a Service
- Fintech
- India
- KYC
- Ledger
- Payments
- UPI
- Virtual Accounts
---
