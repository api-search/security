---
api_specs:
- filename: qoala-authentication-api-openapi.yml
  format: yaml
  label: Qoala Authentication API
  slug: qoala-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qoala/refs/heads/main/openapi/qoala-authentication-api-openapi.yml
- filename: qoala-api-specification-api-openapi.yml
  format: yaml
  label: Qoala API Specification API
  slug: qoala-api-specification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qoala/refs/heads/main/openapi/qoala-api-specification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qoala.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: qoala.app
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: qoala.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 15:46:26 2026 GMT
  host: docs.qoala.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 13:35:33 2026 GMT
  host: api.qoala.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qoala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qoala, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qoala
provider_slug: qoala
slug: qoala-domain-security
source_filename: qoala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: docs.qoala.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 15:46:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.qoala.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 13:35:33 2026 GMT\n  hsts: null\ndomains:\n- domain: qoala.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qoala.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qoala/refs/heads/main/security/qoala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Policies
- Claims
- Southeast Asia
- Indonesia
- Financial Services
- Partner API
---
