---
api_specs:
- filename: frontegg-identity-openapi.yml
  format: yaml
  label: Frontegg Authentication and Identity Management API
  slug: frontegg-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-identity-openapi.yml
- filename: frontegg-tenants-openapi.yml
  format: yaml
  label: Frontegg Account Management API
  slug: frontegg-tenants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-tenants-openapi.yml
- filename: frontegg-sso-openapi.yml
  format: yaml
  label: Frontegg Single Sign-On API
  slug: frontegg-sso
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-sso-openapi.yml
- filename: frontegg-scim-openapi.yml
  format: yaml
  label: Frontegg SCIM Provisioning API
  slug: frontegg-scim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-scim-openapi.yml
- filename: frontegg-entitlements-openapi.yml
  format: yaml
  label: Frontegg Entitlements API
  slug: frontegg-entitlements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-entitlements-openapi.yml
- filename: frontegg-entitlements-agent-openapi.yml
  format: yaml
  label: Frontegg Entitlements Agent (PDP)
  slug: frontegg-entitlements-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-entitlements-agent-openapi.yml
- filename: frontegg-applications-openapi.yml
  format: yaml
  label: Frontegg Multi-Apps API
  slug: frontegg-applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-applications-openapi.yml
- filename: frontegg-audits-openapi.yml
  format: yaml
  label: Frontegg Audits API
  slug: frontegg-audits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-audits-openapi.yml
- filename: frontegg-env-auth-openapi.yml
  format: yaml
  label: Frontegg Environment Authentication API
  slug: frontegg-env-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-env-auth-openapi.yml
- filename: frontegg-combined-openapi.yml
  format: yaml
  label: Frontegg Combined API
  slug: frontegg-combined
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-combined-openapi.yml
- filename: frontegg-webhooks-asyncapi.yml
  format: yaml
  label: Frontegg Webhooks
  slug: frontegg-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/asyncapi/frontegg-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: frontegg.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: frontegg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 17:51:53 2026 GMT
  host: developers.frontegg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.frontegg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frontegg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frontegg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Frontegg
provider_slug: frontegg
slug: frontegg-domain-security
source_filename: frontegg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\n- host: developers.frontegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 17:51:53 2026 GMT\n  hsts: false\n- host: api.frontegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: frontegg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/security/frontegg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Authentication
- Authorization
- Identity Management
- CIAM
- B2B SaaS
- Multi-Tenancy
- RBAC
- SSO
- SCIM
- Entitlements
- OAuth
- OpenID Connect
---
