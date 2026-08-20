---
api_specs:
- filename: sso-authentication-api-openapi.yml
  format: yaml
  label: SSO Authentication API
  slug: sso-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-authentication-api-openapi.yml
- filename: sso-authorization-api-openapi.yml
  format: yaml
  label: SSO Authorization API
  slug: sso-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-authorization-api-openapi.yml
- filename: sso-discovery-api-openapi.yml
  format: yaml
  label: SSO Discovery API
  slug: sso-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-discovery-api-openapi.yml
- filename: sso-keys-api-openapi.yml
  format: yaml
  label: SSO Keys API
  slug: sso-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-keys-api-openapi.yml
- filename: sso-logout-api-openapi.yml
  format: yaml
  label: SSO Logout API
  slug: sso-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-logout-api-openapi.yml
- filename: sso-metadata-api-openapi.yml
  format: yaml
  label: SSO Metadata API
  slug: sso-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-metadata-api-openapi.yml
- filename: sso-token-api-openapi.yml
  format: yaml
  label: SSO Token API
  slug: sso-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-token-api-openapi.yml
- filename: sso-user-info-api-openapi.yml
  format: yaml
  label: SSO User Info API
  slug: sso-user-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-user-info-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oasis-open.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openid.net
  spf: true
hosts:
- cert_expires: Sep  3 09:37:11 2026 GMT
  host: www.oasis-open.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 11:30:22 2026 GMT
  host: openid.net
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SSO, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SSO
provider_slug: sso
slug: sso-domain-security
source_filename: sso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oasis-open.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:37:11 2026 GMT\n  hsts: false\n- host: openid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: oasis-open.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openid.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/security/sso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- OIDC
- SAML
- Security
- Single Sign-On
- SSO
---
