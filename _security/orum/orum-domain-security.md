---
api_specs:
- filename: orum-authentication-api-openapi.yml
  format: yaml
  label: Orum Authentication API
  slug: orum-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-authentication-api-openapi.yml
- filename: orum-balance-api-openapi.yml
  format: yaml
  label: Orum Balance API
  slug: orum-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-balance-api-openapi.yml
- filename: orum-book-transfers-api-openapi.yml
  format: yaml
  label: Orum Book Transfers API
  slug: orum-book-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-book-transfers-api-openapi.yml
- filename: orum-businesses-api-openapi.yml
  format: yaml
  label: Orum Businesses API
  slug: orum-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-businesses-api-openapi.yml
- filename: orum-cards-api-openapi.yml
  format: yaml
  label: Orum Cards API
  slug: orum-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-cards-api-openapi.yml
- filename: orum-configure-webhooks-api-openapi.yml
  format: yaml
  label: Orum Configure webhooks API
  slug: orum-configure-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-configure-webhooks-api-openapi.yml
- filename: orum-eligibility-api-openapi.yml
  format: yaml
  label: Orum Eligibility API
  slug: orum-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-eligibility-api-openapi.yml
- filename: orum-external-accounts-api-openapi.yml
  format: yaml
  label: Orum External Accounts API
  slug: orum-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-external-accounts-api-openapi.yml
- filename: orum-persons-api-openapi.yml
  format: yaml
  label: Orum Persons API
  slug: orum-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-persons-api-openapi.yml
- filename: orum-reports-api-openapi.yml
  format: yaml
  label: Orum Reports API
  slug: orum-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-reports-api-openapi.yml
- filename: orum-schedules-api-openapi.yml
  format: yaml
  label: Orum Schedules API
  slug: orum-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-schedules-api-openapi.yml
- filename: orum-secure-webhooks-api-openapi.yml
  format: yaml
  label: Orum Secure webhooks API
  slug: orum-secure-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-secure-webhooks-api-openapi.yml
- filename: orum-subledgers-api-openapi.yml
  format: yaml
  label: Orum Subledgers API
  slug: orum-subledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-subledgers-api-openapi.yml
- filename: orum-transfer-groups-api-openapi.yml
  format: yaml
  label: Orum Transfer Groups API
  slug: orum-transfer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-transfer-groups-api-openapi.yml
- filename: orum-transfers-api-openapi.yml
  format: yaml
  label: Orum Transfers API
  slug: orum-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-transfers-api-openapi.yml
- filename: orum-trigger-webhooks-api-openapi.yml
  format: yaml
  label: Orum Trigger webhooks API
  slug: orum-trigger-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-trigger-webhooks-api-openapi.yml
- filename: orum-verify-api-openapi.yml
  format: yaml
  label: Orum Verify API
  slug: orum-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: orum.io
  spf: true
hosts:
- cert_expires: Aug 28 03:32:51 2026 GMT
  host: orum.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 03:32:51 2026 GMT
  host: api-sandbox.orum.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: vault.api-sandbox.orum.io
  https: false
kind: domain-security
layout: security
method: probed
name: Orum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orum, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Orum
provider_slug: orum
slug: orum-domain-security
source_filename: orum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:32:51 2026 GMT\n  hsts: null\n- host: api-sandbox.orum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:32:51 2026 GMT\n  hsts: null\n- host: vault.api-sandbox.orum.io\n  https: false\ndomains:\n- domain: orum.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/security/orum-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Payments
- Fintech
- Banking
- Instant Payments
- ACH
- Money Movement
- Bank Account Verification
---
