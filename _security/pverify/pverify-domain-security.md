---
api_specs:
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Eligibility Inquiry API
  slug: eligibility-inquiry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Eligibility Summary API
  slug: eligibility-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Batch Eligibility API
  slug: batch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Claim Status API
  slug: claim-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Payers API
  slug: payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Estimation API
  slug: estimation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pverify.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pverify.io
  spf: false
hosts:
- cert_expires: Sep 17 05:56:56 2026 GMT
  host: www.pverify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:44:14 2026 GMT
  host: docs.pverify.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.pverify.com
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pverify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pVerify, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: pVerify
provider_slug: pverify
slug: pverify-domain-security
source_filename: pverify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:56:56 2026 GMT\n  hsts: false\n- host: docs.pverify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:44:14 2026 GMT\n  hsts: null\n- host: api.pverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: pverify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pverify.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/security/pverify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- 270/271
---
