---
api_specs:
- filename: 1kosmos-access-code-api-openapi.yml
  format: yaml
  label: 1Kosmos Access Code API
  slug: 1kosmos-access-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-access-code-api-openapi.yml
- filename: 1kosmos-ial-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL API
  slug: 1kosmos-ial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial-api-openapi.yml
- filename: 1kosmos-ial2-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL2 API
  slug: 1kosmos-ial2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial2-api-openapi.yml
- filename: 1kosmos-id-verification-api-openapi.yml
  format: yaml
  label: 1Kosmos ID Verification API
  slug: 1kosmos-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-id-verification-api-openapi.yml
- filename: 1kosmos-otp-api-openapi.yml
  format: yaml
  label: 1Kosmos OTP API
  slug: 1kosmos-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-otp-api-openapi.yml
- filename: 1kosmos-reports-api-openapi.yml
  format: yaml
  label: 1Kosmos Reports API
  slug: 1kosmos-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-reports-api-openapi.yml
- filename: 1kosmos-set-up-api-openapi.yml
  format: yaml
  label: 1Kosmos Set up API
  slug: 1kosmos-set-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-set-up-api-openapi.yml
- filename: 1kosmos-user-management-api-openapi.yml
  format: yaml
  label: 1Kosmos User Management API
  slug: 1kosmos-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-user-management-api-openapi.yml
- filename: 1kosmos-verifiable-credentials-api-openapi.yml
  format: yaml
  label: 1Kosmos Verifiable Credentials API
  slug: 1kosmos-verifiable-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-verifiable-credentials-api-openapi.yml
- filename: 1kosmos-workflow-api-api-openapi.yml
  format: yaml
  label: 1Kosmos Workflow API API
  slug: 1kosmos-workflow-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-workflow-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 1kosmos.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: 1kosmos.net
  spf: true
hosts:
- cert_expires: Oct 23 01:10:33 2026 GMT
  host: www.1kosmos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 21:41:21 2026 GMT
  host: developer.1kosmos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 21:30:14 2026 GMT
  host: blockid-trial.1kosmos.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Kosmos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Kosmos, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 1Kosmos
provider_slug: 1kosmos
slug: 1kosmos-domain-security
source_filename: 1kosmos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1kosmos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 01:10:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.1kosmos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:41:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blockid-trial.1kosmos.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1kosmos.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 1kosmos.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/security/1kosmos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity
- Authentication
- Identity Verification
- Passwordless
- Biometrics
- Verifiable Credentials
- FIDO2
- Security
- Company
---
