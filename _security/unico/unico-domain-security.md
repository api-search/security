---
api_specs:
- filename: unico-api-integration.postman_collection.json
  format: json
  label: Unico IDCloud API
  slug: idcloud-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-api-integration.postman_collection.json
- filename: unico-web-sdk-integration.postman_collection.json
  format: json
  label: Unico IDCloud Web & SDK API
  slug: idcloud-web-sdk
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-web-sdk-integration.postman_collection.json
- filename: unico-oauth2.postman_collection.json
  format: json
  label: Unico Identity OAuth2
  slug: identity-oauth2
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-oauth2.postman_collection.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unico.io
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: false
  dnssec: false
  domain: unico.app
  spf: false
hosts:
- cert_expires: Oct 10 17:47:06 2026 GMT
  host: www.unico.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 22:18:02 2026 GMT
  host: developer.unico.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 15:02:26 2026 GMT
  host: api.id.unico.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unico, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unico
provider_slug: unico
slug: unico-domain-security
source_filename: unico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unico.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:47:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.unico.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.id.unico.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 15:02:26 2026 GMT\n  hsts: null\ndomains:\n- domain: unico.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: unico.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"\
  globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/security/unico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Biometrics
- Facial Recognition
- Liveness Detection
- KYC
- Fraud Prevention
- Onboarding
- Authentication
- AML
- Age Verification
- Document Verification
- Identity
- Brazil
- Latin America
---
