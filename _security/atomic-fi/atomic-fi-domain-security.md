---
api_specs:
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Access Tokens API
  slug: atomic-fi-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Transact SDK
  slug: atomic-fi-transact-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Tasks API
  slug: atomic-fi-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Deposit API
  slug: atomic-fi-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Verify API
  slug: atomic-fi-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic PayLink API
  slug: atomic-fi-paylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Data & Transactions API
  slug: atomic-fi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Webhooks API
  slug: atomic-fi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atomicfi.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: atomicfi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: docs.atomicfi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.atomicfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomic Fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Atomic
provider_slug: atomic-fi
slug: atomic-fi-domain-security
source_filename: atomic-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomicfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: docs.atomicfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\n- host: api.atomicfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: atomicfi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/security/atomic-fi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fintech
- Payroll
- Direct Deposit
- Income Verification
- Employment Verification
- Financial Connectivity
- Embedded Finance
---
