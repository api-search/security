---
api_specs:
- filename: telefonica-device-roaming-api-openapi.yml
  format: yaml
  label: Telefónica Device Roaming API
  slug: telefonica-device-roaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-device-roaming-api-openapi.yml
- filename: telefonica-kyc-match-api-openapi.yml
  format: yaml
  label: Telefónica KYC Match API
  slug: telefonica-kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-kyc-match-api-openapi.yml
- filename: telefonica-location-verification-api-openapi.yml
  format: yaml
  label: Telefónica Location Verification API
  slug: telefonica-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-location-verification-api-openapi.yml
- filename: telefonica-number-verification-api-openapi.yml
  format: yaml
  label: Telefónica Number Verification API
  slug: telefonica-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-number-verification-api-openapi.yml
- filename: telefonica-qod-sessions-api-openapi.yml
  format: yaml
  label: Telefónica QoD Sessions API
  slug: telefonica-qod-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-qod-sessions-api-openapi.yml
- filename: telefonica-sim-swap-api-openapi.yml
  format: yaml
  label: Telefónica SIM Swap API
  slug: telefonica-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-sim-swap-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: telefonica.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: opengateway.telefonica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: sandbox.opengateway.telefonica.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telefonica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telefónica, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telefónica
provider_slug: telefonica
slug: telefonica-domain-security
source_filename: telefonica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opengateway.telefonica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.opengateway.telefonica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: telefonica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/security/telefonica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Mobile Network
- CAMARA
- Open Gateway
- Authentication
- Fraud Prevention
- Location Services
---
