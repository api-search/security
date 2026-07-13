---
api_specs:
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Verify Verifications API
  slug: telnyx-verify-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Verify Profiles API
  slug: telnyx-verify-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Number Lookup API
  slug: telnyx-verify-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "alphassl.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@telnyx.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telnyx.com
  spf: true
hosts:
- cert_expires: Oct 31 13:43:45 2026 GMT
  host: telnyx.com
  hsts: false
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:35:03 2026 GMT
  host: developers.telnyx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 10:27:40 2026 GMT
  host: api.telnyx.com
  hsts: false
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telnyx Verify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telnyx Verify API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Telnyx Verify API
provider_slug: telnyx-verify
slug: telnyx-verify-domain-security
source_filename: telnyx-verify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telnyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 13:43:45 2026 GMT\n  hsts: false\n  hsts_max_age: 0\n- host: developers.telnyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:35:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.telnyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:27:40 2026 GMT\n  hsts: false\n  hsts_max_age: 0\ndomains:\n- domain: telnyx.com\n  dnssec: false\n  caa:\n  - '0 issue \"alphassl.com\"'\n  - '0 issue \"digicert.com\"'\n  - '0 iodef \"mailto:security@telnyx.com\"'\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/security/telnyx-verify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Number Verification
- Phone Verification
- OTP
- 2FA
- Lookup
- Verify
- Number Lookup
- CNAM
- Identity
- Anti-Fraud
---
