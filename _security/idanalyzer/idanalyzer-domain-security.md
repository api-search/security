---
api_specs:
- filename: idanalyzer-account-api-openapi.yml
  format: yaml
  label: ID Analyzer Account API
  slug: idanalyzer-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-account-api-openapi.yml
- filename: idanalyzer-aml-api-openapi.yml
  format: yaml
  label: ID Analyzer AML API
  slug: idanalyzer-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-aml-api-openapi.yml
- filename: idanalyzer-biometric-api-openapi.yml
  format: yaml
  label: ID Analyzer Biometric API
  slug: idanalyzer-biometric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-biometric-api-openapi.yml
- filename: idanalyzer-contract-api-openapi.yml
  format: yaml
  label: ID Analyzer Contract API
  slug: idanalyzer-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-contract-api-openapi.yml
- filename: idanalyzer-docupass-api-openapi.yml
  format: yaml
  label: ID Analyzer Docupass API
  slug: idanalyzer-docupass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-docupass-api-openapi.yml
- filename: idanalyzer-profile-api-openapi.yml
  format: yaml
  label: ID Analyzer Profile API
  slug: idanalyzer-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-profile-api-openapi.yml
- filename: idanalyzer-scanner-api-openapi.yml
  format: yaml
  label: ID Analyzer Scanner API
  slug: idanalyzer-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-scanner-api-openapi.yml
- filename: idanalyzer-transaction-api-openapi.yml
  format: yaml
  label: ID Analyzer Transaction API
  slug: idanalyzer-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-transaction-api-openapi.yml
- filename: idanalyzer-webhook-api-openapi.yml
  format: yaml
  label: ID Analyzer Webhook API
  slug: idanalyzer-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: idanalyzer.com
  spf: true
hosts:
- cert_expires: Oct  3 09:16:20 2026 GMT
  host: www.idanalyzer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 01:41:04 2026 GMT
  host: developer.idanalyzer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:16:20 2026 GMT
  host: api2.idanalyzer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Idanalyzer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ID Analyzer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ID Analyzer
provider_slug: idanalyzer
slug: idanalyzer-domain-security
source_filename: idanalyzer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.idanalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:16:20 2026 GMT\n  hsts: false\n- host: developer.idanalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:41:04 2026 GMT\n  hsts: false\n- host: api2.idanalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:16:20 2026 GMT\n  hsts: null\ndomains:\n- domain: idanalyzer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/security/idanalyzer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity Verification
- KYC
- AML
- Document OCR
- Biometrics
- Face Matching
- Fraud Detection
- Passport
- Driver License
- Liveness Detection
---
