---
api_specs:
- filename: logto-openapi-original.yml
  format: yaml
  label: Logto API
  slug: logto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logto/refs/heads/main/openapi/logto-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logto.io
  spf: true
hosts:
- cert_expires: Aug 30 23:01:06 2026 GMT
  host: logto.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 22:48:15 2026 GMT
  host: docs.logto.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Logto
provider_slug: logto
slug: logto-domain-security
source_filename: logto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:01:06 2026 GMT\n  hsts: false\n- host: docs.logto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:48:15 2026 GMT\n  hsts: false\ndomains:\n- domain: logto.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logto/refs/heads/main/security/logto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Authentication
- Authorization
- Identity
- OIDC
- OAuth
- SAML
- Open Source
---
