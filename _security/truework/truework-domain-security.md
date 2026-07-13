---
api_specs:
- filename: truework-verifications-orders-openapi.yml
  format: yaml
  label: Truework Verifications API
  slug: truework-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-verifications-orders-openapi.yml
- filename: truework-beta-openapi.yml
  format: yaml
  label: Truework Qualifications API (Beta)
  slug: truework-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-beta-openapi.yml
- filename: truework-beta-openapi.yml
  format: yaml
  label: Truework Tenant Properties API (Beta)
  slug: truework-tenant-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-beta-openapi.yml
- filename: truework-webhooks-openapi.yml
  format: yaml
  label: Truework Webhooks
  slug: truework-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truework.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.truework.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.truework.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: js.truework.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truework, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truework
provider_slug: truework
slug: truework-domain-security
source_filename: truework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.truework.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: js.truework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: truework.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/security/truework-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Verifications
- Income Verification
- Employment Verification
- VOIE
- Mortgage
- Lending
- Credit Unions
- Identity
- KYC
- Fintech
---
