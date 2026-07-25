---
api_specs:
- filename: smile-identity-authentication-api-openapi.yml
  format: yaml
  label: Smile Identity Authentication API
  slug: smile-identity-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-authentication-api-openapi.yml
- filename: smile-identity-biometric-authentication-api-openapi.yml
  format: yaml
  label: Smile Identity Biometric Authentication API
  slug: smile-identity-biometric-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-biometric-authentication-api-openapi.yml
- filename: smile-identity-biometric-enrollment-api-openapi.yml
  format: yaml
  label: Smile Identity Biometric Enrollment API
  slug: smile-identity-biometric-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-biometric-enrollment-api-openapi.yml
- filename: smile-identity-biometric-kyc-api-openapi.yml
  format: yaml
  label: Smile Identity Biometric KYC API
  slug: smile-identity-biometric-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-biometric-kyc-api-openapi.yml
- filename: smile-identity-callback-replay-api-openapi.yml
  format: yaml
  label: Smile Identity Callback Replay API
  slug: smile-identity-callback-replay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-callback-replay-api-openapi.yml
- filename: smile-identity-document-verification-api-openapi.yml
  format: yaml
  label: Smile Identity Document Verification API
  slug: smile-identity-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-document-verification-api-openapi.yml
- filename: smile-identity-enhanced-document-verification-api-openapi.yml
  format: yaml
  label: Smile Identity Enhanced Document Verification API
  slug: smile-identity-enhanced-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-enhanced-document-verification-api-openapi.yml
- filename: smile-identity-enhanced-kyc-api-openapi.yml
  format: yaml
  label: Smile Identity Enhanced KYC API
  slug: smile-identity-enhanced-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-enhanced-kyc-api-openapi.yml
- filename: smile-identity-services-api-openapi.yml
  format: yaml
  label: Smile Identity Services API
  slug: smile-identity-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-services-api-openapi.yml
- filename: smile-identity-smart-selfie-compare-api-openapi.yml
  format: yaml
  label: Smile Identity Smart Selfie Compare API
  slug: smile-identity-smart-selfie-compare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-smart-selfie-compare-api-openapi.yml
- filename: smile-identity-users-api-openapi.yml
  format: yaml
  label: Smile Identity Users API
  slug: smile-identity-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-users-api-openapi.yml
- filename: smile-identity-verification-status-api-openapi.yml
  format: yaml
  label: Smile Identity Verification Status API
  slug: smile-identity-verification-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-verification-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usesmileid.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smileidentity.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: usesmileid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:11:34 2026 GMT
  host: docs.usesmileid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:29:57 2026 GMT
  host: api.smileidentity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smile Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smile Identity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smile Identity
provider_slug: smile-identity
slug: smile-identity-domain-security
source_filename: smile-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usesmileid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.usesmileid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:11:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smileidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:29:57 2026 GMT\n  hsts: null\ndomains:\n- domain: usesmileid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smileidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/security/smile-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity Verification
- KYC
- KYB
- Biometrics
- Liveness Detection
- Document Verification
- AML
- Fraud Prevention
- Compliance
- Onboarding
- Africa
---
