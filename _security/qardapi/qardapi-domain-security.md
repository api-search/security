---
api_specs:
- filename: qardapi-openapi-generated.yml
  format: yaml
  label: Qard API
  slug: qardapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qardapi/openapi/_ae-authored/qardapi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qardapi.com
  spf: true
hosts:
- host: qardapi.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''qardapi.com'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qardapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qard
provider_slug: qardapi
slug: qardapi-domain-security
source_filename: qardapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qardapi.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''qardapi.com'\n  hsts: null\ndomains:\n- domain: qardapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/qardapi/security/qardapi-domain-security.yml
summary_line: DMARC
tags:
- Company
---
