---
api_specs:
- filename: farofinance-app-api-openapi.json
  format: json
  label: Faro Api API
  slug: faro-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/_original/farofinance-app-api-openapi.json
description: ''
domains:
- caa:
  - t37m4jt6.up.railway.app.
  dmarc: false
  dnssec: true
  domain: farofinance.app
  spf: false
hosts:
- host: farofinance.app
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''farofinance'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Faro
provider_slug: farofinance-app
slug: farofinance-app-domain-security
source_filename: farofinance-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farofinance.app\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''farofinance'\n  hsts: null\ndomains:\n- domain: farofinance.app\n  dnssec: true\n  caa:\n  - t37m4jt6.up.railway.app.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/farofinance-app/security/farofinance-app-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Security
- Fraud Prevention
- Verification
- Payments
---
