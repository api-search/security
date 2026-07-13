---
api_specs:
- filename: clerk-backend-api-openapi.yml
  format: yaml
  label: Clerk Backend API
  slug: clerk-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-backend-api-openapi.yml
- filename: clerk-frontend-api-openapi.yml
  format: yaml
  label: Clerk Frontend API
  slug: clerk-frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-frontend-api-openapi.yml
- filename: clerk-platform-api-openapi.yml
  format: yaml
  label: Clerk Platform API
  slug: clerk-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-platform-api-openapi.yml
- filename: clerk-webhooks-openapi.yml
  format: yaml
  label: Clerk Webhooks
  slug: clerk-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-webhooks-openapi.yml
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
  domain: clerk.dev
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
- cert_expires: Sep 30 18:43:13 2026 GMT
  host: api.clerk.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clerk Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clerk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clerk
provider_slug: clerk-com
slug: clerk-com-domain-security
source_filename: clerk-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clerk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:08:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.clerk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:39:49 2026 GMT\n  hsts: null\n- host: api.clerk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:43:13 2026 GMT\n  hsts: null\ndomains:\n- domain: clerk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clerk.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/security/clerk-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- B2B SaaS
- CIAM
- Identity Management
- MFA
- OAuth
- OpenID Connect
- Organizations
- Passkeys
- SAML
- Security
- Sessions
- SSO
- User Management
---
