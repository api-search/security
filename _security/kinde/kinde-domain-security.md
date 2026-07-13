---
api_specs:
- filename: kinde-management-api-openapi.yml
  format: yaml
  label: Kinde Management API
  slug: kinde-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde/refs/heads/main/openapi/kinde-management-api-openapi.yml
- filename: kinde-frontend-api-openapi.yml
  format: yaml
  label: Kinde Account API
  slug: kinde-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde/refs/heads/main/openapi/kinde-frontend-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kinde.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: docs.kinde.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kinde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinde, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kinde
provider_slug: kinde
slug: kinde-domain-security
source_filename: kinde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.kinde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kinde.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinde/refs/heads/main/security/kinde-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Authorization
- Customer Identity
- Identity Management
- OAuth
- OpenID Connect
- Single Sign-On
- Multi-Factor Authentication
- Role-Based Access Control
- Feature Flags
- Billing
- B2B
- SaaS
- Developer Platform
---
