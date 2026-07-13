---
api_specs:
- filename: onelogin-openapi.yml
  format: yaml
  label: OneLogin API
  slug: onelogin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onelogin/refs/heads/main/openapi/onelogin-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onelogin.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.onelogin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: developers.onelogin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: <subdomain>.onelogin.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<subdomain>'
kind: domain-security
layout: security
method: probed
name: Onelogin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneLogin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OneLogin
provider_slug: onelogin
slug: onelogin-domain-security
source_filename: onelogin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onelogin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.onelogin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <subdomain>.onelogin.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<subdomain>'\n  hsts: null\ndomains:\n- domain: onelogin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onelogin/refs/heads/main/security/onelogin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Access Management
- Single Sign-On
- Multi-Factor Authentication
- SAML
- OAuth
---
