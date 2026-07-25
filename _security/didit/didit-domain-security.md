---
api_specs:
- filename: didit-billing-api-openapi.yml
  format: yaml
  label: Didit Billing API
  slug: didit-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-billing-api-openapi.yml
- filename: didit-businesses-api-openapi.yml
  format: yaml
  label: Didit Businesses API
  slug: didit-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-businesses-api-openapi.yml
- filename: didit-case-blueprints-api-openapi.yml
  format: yaml
  label: Didit Case Blueprints API
  slug: didit-case-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-case-blueprints-api-openapi.yml
- filename: didit-cases-api-openapi.yml
  format: yaml
  label: Didit Cases API
  slug: didit-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-cases-api-openapi.yml
- filename: didit-customization-api-openapi.yml
  format: yaml
  label: Didit Customization API
  slug: didit-customization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-customization-api-openapi.yml
- filename: didit-questionnaires-api-openapi.yml
  format: yaml
  label: Didit Questionnaires API
  slug: didit-questionnaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-questionnaires-api-openapi.yml
- filename: didit-regulatory-reports-api-openapi.yml
  format: yaml
  label: Didit Regulatory Reports API
  slug: didit-regulatory-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-regulatory-reports-api-openapi.yml
- filename: didit-report-templates-api-openapi.yml
  format: yaml
  label: Didit Report Templates API
  slug: didit-report-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-report-templates-api-openapi.yml
- filename: didit-session-api-openapi.yml
  format: yaml
  label: Didit Session API
  slug: didit-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-session-api-openapi.yml
- filename: didit-sessions-api-openapi.yml
  format: yaml
  label: Didit Sessions API
  slug: didit-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-sessions-api-openapi.yml
- filename: didit-standalone-apis-api-openapi.yml
  format: yaml
  label: Didit Standalone APIs API
  slug: didit-standalone-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-standalone-apis-api-openapi.yml
- filename: didit-system-api-openapi.yml
  format: yaml
  label: Didit System API
  slug: didit-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-system-api-openapi.yml
- filename: didit-transactions-api-openapi.yml
  format: yaml
  label: Didit Transactions API
  slug: didit-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-transactions-api-openapi.yml
- filename: didit-travel-rule-api-openapi.yml
  format: yaml
  label: Didit Travel Rule API
  slug: didit-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-travel-rule-api-openapi.yml
- filename: didit-users-api-openapi.yml
  format: yaml
  label: Didit Users API
  slug: didit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-users-api-openapi.yml
- filename: didit-webhook-api-openapi.yml
  format: yaml
  label: Didit Webhook API
  slug: didit-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-webhook-api-openapi.yml
- filename: didit-workflows-api-openapi.yml
  format: yaml
  label: Didit Workflows API
  slug: didit-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: didit.me
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: verification.didit.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Didit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Didit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Didit
provider_slug: didit
slug: didit-domain-security
source_filename: didit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verification.didit.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: didit.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/security/didit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Compliance
- Biometrics
- Transaction Monitoring
- Crypto
---
