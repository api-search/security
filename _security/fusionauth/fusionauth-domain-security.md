---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: FusionAuth API
  slug: fusionauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/FusionAuth/fusionauth-openapi/main/openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fusionauth.io
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: fusionauth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: sandbox.fusionauth.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fusionauth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FusionAuth, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FusionAuth
provider_slug: fusionauth
slug: fusionauth-domain-security
source_filename: fusionauth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fusionauth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.fusionauth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fusionauth.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusionauth/refs/heads/main/security/fusionauth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- CIAM
- OAuth
- OpenID Connect
- Single Sign-On
- Multi-Factor Authentication
---
