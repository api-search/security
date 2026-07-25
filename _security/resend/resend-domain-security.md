---
api_specs:
- filename: resend-apis-api-openapi.yml
  format: yaml
  label: Resend Apis API
  slug: resend-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-apis-api-openapi.yml
- filename: resend-audience-api-openapi.yml
  format: yaml
  label: Resend Audience API
  slug: resend-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-audience-api-openapi.yml
- filename: resend-audiences-api-openapi.yml
  format: yaml
  label: Resend Audiences API
  slug: resend-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-audiences-api-openapi.yml
- filename: resend-batch-api-openapi.yml
  format: yaml
  label: Resend Batch API
  slug: resend-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-batch-api-openapi.yml
- filename: resend-broadcasts-api-openapi.yml
  format: yaml
  label: Resend Broadcasts API
  slug: resend-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-broadcasts-api-openapi.yml
- filename: resend-cancel-api-openapi.yml
  format: yaml
  label: Resend Cancel API
  slug: resend-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-cancel-api-openapi.yml
- filename: resend-contacts-api-openapi.yml
  format: yaml
  label: Resend Contacts API
  slug: resend-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-contacts-api-openapi.yml
- filename: resend-domains-api-openapi.yml
  format: yaml
  label: Resend Domains API
  slug: resend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-domains-api-openapi.yml
- filename: resend-email-api-openapi.yml
  format: yaml
  label: Resend Email API
  slug: resend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-email-api-openapi.yml
- filename: resend-emails-api-openapi.yml
  format: yaml
  label: Resend Emails API
  slug: resend-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-emails-api-openapi.yml
- filename: resend-keys-api-openapi.yml
  format: yaml
  label: Resend Keys API
  slug: resend-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-keys-api-openapi.yml
- filename: resend-send-api-openapi.yml
  format: yaml
  label: Resend Send API
  slug: resend-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-send-api-openapi.yml
- filename: resend-verify-api-openapi.yml
  format: yaml
  label: Resend Verify API
  slug: resend-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: resend.com
  spf: true
hosts:
- cert_expires: Sep 28 17:52:04 2026 GMT
  host: resend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 13:48:19 2026 GMT
  host: api.resend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Resend
provider_slug: resend
slug: resend-domain-security
source_filename: resend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:52:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.resend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 13:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: resend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/security/resend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Developer Tools
- Transactional Email
- Marketing Email
---
