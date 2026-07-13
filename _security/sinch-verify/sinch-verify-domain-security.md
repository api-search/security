---
api_specs:
- filename: sinch-verify-openapi.yml
  format: yaml
  label: Sinch Start Verification API
  slug: sinch-verify-start-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/openapi/sinch-verify-openapi.yml
- filename: sinch-verify-openapi.yml
  format: yaml
  label: Sinch Report Verification API
  slug: sinch-verify-report-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/openapi/sinch-verify-openapi.yml
- filename: sinch-verify-openapi.yml
  format: yaml
  label: Sinch Verification Status API
  slug: sinch-verify-verification-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/openapi/sinch-verify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sinch.com
  spf: true
hosts:
- cert_expires: Oct  9 21:47:21 2026 GMT
  host: sinch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:01:41 2026 GMT
  host: developers.sinch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: verification.api.sinch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sinch Verify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sinch Verification API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sinch Verification API
provider_slug: sinch-verify
slug: sinch-verify-domain-security
source_filename: sinch-verify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sinch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 21:47:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.sinch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:01:41 2026 GMT\n  hsts: false\n- host: verification.api.sinch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sinch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/security/sinch-verify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Number Verification
- Phone Verification
- OTP
- 2FA
- CPaaS
- SMS Verification
- Flash Call
- Two-Factor Authentication
- Identity Verification
- Sinch
---
