---
api_specs:
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge KYC OCR API
  slug: hyperverge-kyc-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Database Verification API
  slug: hyperverge-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Input Validation API
  slug: hyperverge-input-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Matching API
  slug: hyperverge-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Face Match API
  slug: hyperverge-face-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hyperverge.co
  spf: true
  spf_policy: -all (hard fail)
hosts:
- cert_expires: Aug 31 03:10:52 2026 GMT
  cert_issuer: Let's Encrypt
  host: hyperverge.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: LiteSpeed
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  cert_issuer: Amazon
  host: documentation.hyperverge.co
  hsts: false
  https: true
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Jul 15 02:21:43 2026 GMT
  cert_issuer: GoDaddy
  host: ind-docs.hyperverge.co
  hsts: false
  https: true
  note: Root path returns HTTP 502 (endpoints require appId/appKey and a valid request body).
  server: awselb/2.0
  tls_version: TLSv1.2
- cert_expires: Jan  3 03:46:05 2027 GMT
  cert_issuer: GoDaddy
  host: ind-verify.hyperverge.co
  hsts: false
  https: true
  note: Root path returns HTTP 502; GET /api returns "Aok".
  server: awselb/2.0
  tls_version: TLSv1.2
- cert_expires: Jul 15 02:21:43 2026 GMT
  cert_issuer: GoDaddy
  host: ind-faceid.hyperverge.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  server: nginx
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hyperverge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HyperVerge, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HyperVerge
provider_slug: hyperverge
slug: hyperverge-domain-security
source_filename: hyperverge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + REST API hosts\nhosts:\n- host: hyperverge.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Aug 31 03:10:52 2026 GMT\n  server: LiteSpeed\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: documentation.hyperverge.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  server: AmazonS3\n  hsts: false\n- host: ind-docs.hyperverge.co\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GoDaddy\n  cert_expires: Jul 15 02:21:43 2026 GMT\n  server: awselb/2.0\n  hsts: false\n  note: Root path returns HTTP 502 (endpoints require appId/appKey and a valid request body).\n- host: ind-verify.hyperverge.co\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GoDaddy\n  cert_expires: Jan  3 03:46:05 2027 GMT\n  server: awselb/2.0\n  hsts: false\n  note:\
  \ Root path returns HTTP 502; GET /api returns \"Aok\".\n- host: ind-faceid.hyperverge.co\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GoDaddy\n  cert_expires: Jul 15 02:21:43 2026 GMT\n  server: nginx\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: hyperverge.co\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all (hard fail)'\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/security/hyperverge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- KYC
- Face Authentication
- Liveness
- Document Verification
- India
- AML
- Onboarding
- Fraud Prevention
- AI
---
