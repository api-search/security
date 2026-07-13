---
api_specs:
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Users API
  slug: clerk-dev-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Organizations API
  slug: clerk-dev-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Organization Memberships API
  slug: clerk-dev-organization-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Organization Invitations API
  slug: clerk-dev-organization-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Sessions API
  slug: clerk-dev-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Clients API
  slug: clerk-dev-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Sign-ups & Sign-in Tokens API
  slug: clerk-dev-sign-ups-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk JWT Templates API
  slug: clerk-dev-jwt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk JWKS API
  slug: clerk-dev-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Email & SMS API
  slug: clerk-dev-email-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Allowlist & Blocklist API
  slug: clerk-dev-allowlist-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Invitations API
  slug: clerk-dev-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk SAML & Enterprise Connections API
  slug: clerk-dev-saml-enterprise-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk OAuth Applications API
  slug: clerk-dev-oauth-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
- filename: clerk-dev-openapi.yml
  format: yaml
  label: Clerk Webhooks API
  slug: clerk-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clerk.com
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
kind: domain-security
layout: security
method: probed
name: Clerk Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clerk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clerk
provider_slug: clerk-dev
slug: clerk-dev-domain-security
source_filename: clerk-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clerk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:08:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.clerk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:39:49 2026 GMT\n  hsts: null\ndomains:\n- domain: clerk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/security/clerk-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- User Management
- Identity
- Sessions
- Organizations
- SSO
- JWT
- MFA
---
