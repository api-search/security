---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Casdoor REST API
  slug: casdoor-rest-api
  spec_type: OpenAPI
  url: https://door.casdoor.com/swagger/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: casdoor.org
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: casdoor.ai
  spf: false
hosts:
- cert_expires: Sep  3 14:50:35 2026 GMT
  host: casdoor.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 14:27:25 2026 GMT
  host: casdoor.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 14:38:31 2026 GMT
  host: door.casdoor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Casdoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casdoor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Casdoor
provider_slug: casdoor
slug: casdoor-domain-security
source_filename: casdoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: casdoor.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:50:35 2026 GMT\n  hsts: false\n- host: casdoor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:27:25 2026 GMT\n  hsts: false\n- host: door.casdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:38:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: casdoor.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: casdoor.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/security/casdoor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Authentication
- Authorization
- IAM
- Identity
- LDAP
- MCP
- MFA
- OAuth
- OIDC
- Open Source
- Passkeys
- SAML
- SCIM
- Single Sign-On
- SSO
- WebAuthn
---
