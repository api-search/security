---
api_specs:
- filename: incode-openapi.yml
  format: yaml
  label: Incode Onboarding Sessions API
  slug: incode-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode ID Verification API
  slug: incode-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Face and Liveness API
  slug: incode-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Government Validation API
  slug: incode-government-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Watchlist and AML API
  slug: incode-watchlist-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Results API
  slug: incode-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Webhooks API
  slug: incode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: incode.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: incodesmile.com
  spf: false
hosts:
- cert_expires: Aug 25 00:12:03 2026 GMT
  host: incode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 14:27:11 2026 GMT
  host: developer.incode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: demo-api.incodesmile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incode, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Incode
provider_slug: incode
slug: incode-domain-security
source_filename: incode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:12:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.incode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:27:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo-api.incodesmile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: incode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: incodesmile.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/security/incode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Biometrics
- KYC
- Liveness
- Onboarding
---
