---
api_specs:
- filename: persona-accounts-api-openapi.yml
  format: yaml
  label: Persona Accounts API
  slug: persona-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-accounts-api-openapi.yml
- filename: persona-inquiries-api-openapi.yml
  format: yaml
  label: Persona Inquiries API
  slug: persona-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-inquiries-api-openapi.yml
- filename: persona-lists-api-openapi.yml
  format: yaml
  label: Persona Lists API
  slug: persona-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-lists-api-openapi.yml
- filename: persona-reports-api-openapi.yml
  format: yaml
  label: Persona Reports API
  slug: persona-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-reports-api-openapi.yml
- filename: persona-transactions-api-openapi.yml
  format: yaml
  label: Persona Transactions API
  slug: persona-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-transactions-api-openapi.yml
- filename: persona-verifications-api-openapi.yml
  format: yaml
  label: Persona Verifications API
  slug: persona-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-verifications-api-openapi.yml
- filename: persona-webhooks-api-openapi.yml
  format: yaml
  label: Persona Webhooks API
  slug: persona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: withpersona.com
  spf: true
hosts:
- cert_expires: Aug 23 00:29:30 2026 GMT
  host: withpersona.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 01:41:23 2026 GMT
  host: docs.withpersona.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Persona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Persona, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Persona
provider_slug: persona
slug: persona-domain-security
source_filename: persona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withpersona.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:29:30 2026 GMT\n  hsts: null\n- host: docs.withpersona.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:41:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withpersona.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/security/persona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Identity Verification
- KYC
---
