---
api_specs:
- filename: openapi-specs
  format: yaml
  label: Clerk Backend API
  slug: backend-api
  spec_type: OpenAPI
  url: https://github.com/clerk/openapi-specs
- filename: clerk-webhooks-asyncapi.yml
  format: yaml
  label: Clerk Webhooks (Svix)
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/asyncapi/clerk-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clerk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accounts.dev
  spf: true
hosts:
- cert_expires: Oct  9 02:08:46 2026 GMT
  host: clerk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 15:39:49 2026 GMT
  host: api.clerk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: clerk.accounts.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Clerk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clerk, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clerk
provider_slug: clerk
slug: clerk-domain-security
source_filename: clerk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clerk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:08:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.clerk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:39:49 2026 GMT\n  hsts: null\n- host: clerk.accounts.dev\n  https: false\ndomains:\n- domain: clerk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: accounts.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/security/clerk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- User Management
- Identity
- Passkeys
- MFA
- B2B
- Organizations
- Billing
---
