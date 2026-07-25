---
api_specs:
- filename: accurate-bg-adjudication-api-openapi.yml
  format: yaml
  label: Accurate Background Adjudication API
  slug: accurate-bg-adjudication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-adjudication-api-openapi.yml
- filename: accurate-bg-candidates-api-openapi.yml
  format: yaml
  label: Accurate Background Candidates API
  slug: accurate-bg-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-candidates-api-openapi.yml
- filename: accurate-bg-documents-api-openapi.yml
  format: yaml
  label: Accurate Background Documents API
  slug: accurate-bg-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-documents-api-openapi.yml
- filename: accurate-bg-notifications-api-openapi.yml
  format: yaml
  label: Accurate Background Notifications API
  slug: accurate-bg-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-notifications-api-openapi.yml
- filename: accurate-bg-orders-api-openapi.yml
  format: yaml
  label: Accurate Background Orders API
  slug: accurate-bg-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-orders-api-openapi.yml
- filename: accurate-bg-packages-api-openapi.yml
  format: yaml
  label: Accurate Background Packages API
  slug: accurate-bg-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-packages-api-openapi.yml
- filename: accurate-bg-reports-api-openapi.yml
  format: yaml
  label: Accurate Background Reports API
  slug: accurate-bg-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-reports-api-openapi.yml
- filename: accurate-bg-utility-api-openapi.yml
  format: yaml
  label: Accurate Background Utility API
  slug: accurate-bg-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-utility-api-openapi.yml
- filename: accurate-bg-verifications-api-openapi.yml
  format: yaml
  label: Accurate Background Verifications API
  slug: accurate-bg-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-verifications-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accurate.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Aug 31 01:23:57 2026 GMT
  host: www.accurate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: accurate.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: api.accuratebackground.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Accurate Bg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accurate Background, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Accurate Background
provider_slug: accurate-bg
slug: accurate-bg-domain-security
source_filename: accurate-bg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accurate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: accurate.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.accuratebackground.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: accurate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/security/accurate-bg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Background Checks
- Employment Screening
- Identity Verification
- Compliance
- HR Tech
- Screening
---
