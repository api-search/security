---
api_specs:
- filename: snappt-account-api-openapi.yml
  format: yaml
  label: Snappt Account API
  slug: snappt-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-account-api-openapi.yml
- filename: snappt-applicant-sessions-api-openapi.yml
  format: yaml
  label: Snappt Applicant Sessions API
  slug: snappt-applicant-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-applicant-sessions-api-openapi.yml
- filename: snappt-applicants-api-openapi.yml
  format: yaml
  label: Snappt Applicants API
  slug: snappt-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-applicants-api-openapi.yml
- filename: snappt-id-verification-api-openapi.yml
  format: yaml
  label: Snappt ID Verification API
  slug: snappt-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-id-verification-api-openapi.yml
- filename: snappt-internal-idv-api-openapi.yml
  format: yaml
  label: Snappt Internal IDV API
  slug: snappt-internal-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-internal-idv-api-openapi.yml
- filename: snappt-properties-api-openapi.yml
  format: yaml
  label: Snappt Properties API
  slug: snappt-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-properties-api-openapi.yml
- filename: snappt-webhooks-api-openapi.yml
  format: yaml
  label: Snappt Webhooks API
  slug: snappt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snappt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 26 06:02:14 2026 GMT
  host: snappt.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: snappt-enterprise-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 14:13:46 2026 GMT
  host: enterprise-api.snappt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snappt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snappt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Snappt
provider_slug: snappt
slug: snappt-domain-security
source_filename: snappt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snappt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 06:02:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: snappt-enterprise-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: enterprise-api.snappt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:13:46 2026 GMT\n  hsts: null\ndomains:\n- domain: snappt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/security/snappt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- fraud-detection
- document-verification
- identity-verification
- income-verification
- property-management
- multifamily
- real-estate
- proptech
- tenant-screening
- rental-applications
- webhooks
---
