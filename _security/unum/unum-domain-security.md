---
api_specs:
- filename: unum-authentication-api-openapi.yml
  format: yaml
  label: Unum Authentication API
  slug: unum-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-authentication-api-openapi.yml
- filename: unum-billing-api-openapi.yml
  format: yaml
  label: Unum Billing API
  slug: unum-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-billing-api-openapi.yml
- filename: unum-eligibility-api-openapi.yml
  format: yaml
  label: Unum Eligibility API
  slug: unum-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-eligibility-api-openapi.yml
- filename: unum-enrollment-api-openapi.yml
  format: yaml
  label: Unum Enrollment API
  slug: unum-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-enrollment-api-openapi.yml
- filename: unum-evidence-of-insurability-api-openapi.yml
  format: yaml
  label: Unum Evidence of Insurability API
  slug: unum-evidence-of-insurability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-evidence-of-insurability-api-openapi.yml
- filename: unum-leave-management-api-openapi.yml
  format: yaml
  label: Unum Leave Management API
  slug: unum-leave-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-leave-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unum.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.unum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.unum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.unum.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Unum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unum
provider_slug: unum
slug: unum-domain-security
source_filename: unum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\n- host: developer.unum.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: unum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/security/unum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Benefits Administration
- HR Integration
- Disability Insurance
- Life Insurance
- Fortune 500
---
