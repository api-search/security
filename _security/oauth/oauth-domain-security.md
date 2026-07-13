---
api_specs:
- filename: oauth-token-endpoint.yml
  format: yaml
  label: OAuth 2.0 Authorization Server API
  slug: oauth-2-authorization-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/openapi/oauth-token-endpoint.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oauth.net
  spf: true
hosts:
- cert_expires: Sep  4 13:06:20 2026 GMT
  host: oauth.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oauth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OAuth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OAuth
provider_slug: oauth
slug: oauth-domain-security
source_filename: oauth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oauth.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:06:20 2026 GMT\n  hsts: false\ndomains:\n- domain: oauth.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/security/oauth-domain-security.yml
summary_line: TLSv1.3
tags:
- Access Control
- Authorization
- OAuth
- Security
- Tokens
---
