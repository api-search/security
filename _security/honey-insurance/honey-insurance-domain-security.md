---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: honeyinsurance.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.honeyinsurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 16:58:24 2026 GMT
  host: auth.honeyinsurance.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Auth0 custom-domain tenant serving anonymous OIDC discovery and JWKS.
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.honeyinsurance.com
  hsts: false
  https: true
  note: Private AWS API Gateway backing Honey's own quote funnel and account app. Every anonymous path returns HTTP 403 {"message":"Forbidden"}; no HSTS header is sent on the deny response.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Honey Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honey Insurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Honey Insurance
provider_slug: honey-insurance
slug: honey-insurance-domain-security
source_filename: honey-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.honeyinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: auth.honeyinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:58:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Auth0 custom-domain tenant serving anonymous OIDC discovery and JWKS.\n- host: api.honeyinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Private AWS API Gateway backing Honey's own quote funnel and account app.\n    Every anonymous path returns HTTP 403 {\"message\":\"Forbidden\"}; no HSTS\n    header is sent on the deny response.\ndomains:\n- domain: honeyinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honey-insurance/refs/heads/main/security/honey-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Insurtech
- Home Insurance
- Property and Casualty
- Personal Lines
- Direct to Consumer
- Embedded Insurance
- Smart Home
- Claims
- Underwriting
---
