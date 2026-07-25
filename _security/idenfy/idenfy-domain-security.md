---
api_specs:
- filename: idenfy-fraud-api-openapi.yml
  format: yaml
  label: iDenfy Fraud Prevention API
  slug: idenfy-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-fraud-api-openapi.yml
- filename: idenfy-face-authentication-api-openapi.yml
  format: yaml
  label: iDenfy Face Authentication API
  slug: idenfy-face-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-face-authentication-api-openapi.yml
- filename: idenfy-aml-api-openapi.yml
  format: yaml
  label: iDenfy Aml API
  slug: idenfy-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-aml-api-openapi.yml
- filename: idenfy-bank-api-openapi.yml
  format: yaml
  label: iDenfy Bank API
  slug: idenfy-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-bank-api-openapi.yml
- filename: idenfy-face-authentication-api-openapi.yml
  format: yaml
  label: iDenfy Face Authentication API
  slug: idenfy-face-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-face-authentication-api-openapi.yml
- filename: idenfy-fraud-api-openapi.yml
  format: yaml
  label: iDenfy Fraud API
  slug: idenfy-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-fraud-api-openapi.yml
- filename: idenfy-kyb-api-openapi.yml
  format: yaml
  label: iDenfy Kyb API
  slug: idenfy-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-kyb-api-openapi.yml
- filename: idenfy-kyc-api-openapi.yml
  format: yaml
  label: iDenfy Kyc API
  slug: idenfy-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-kyc-api-openapi.yml
- filename: idenfy-token-api-openapi.yml
  format: yaml
  label: iDenfy Token API
  slug: idenfy-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: idenfy.com
  spf: true
hosts:
- cert_expires: Oct  1 10:31:14 2026 GMT
  host: www.idenfy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 08:18:26 2026 GMT
  host: documentation.idenfy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: ivs.idenfy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Idenfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iDenfy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iDenfy
provider_slug: idenfy
slug: idenfy-domain-security
source_filename: idenfy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.idenfy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.idenfy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:18:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ivs.idenfy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: idenfy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/security/idenfy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AML
- Compliance
- Fraud Detection
- Identity Verification
- KYB
- KYC
---
