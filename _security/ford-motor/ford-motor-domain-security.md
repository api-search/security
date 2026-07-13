---
api_specs:
- filename: ford-motor-ford-api-openapi.yml
  format: yaml
  label: Ford Developer API
  slug: ford-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford-motor/refs/heads/main/openapi/ford-motor-ford-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ford.com
  spf: true
hosts:
- host: developer.ford.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: api.ford.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ford Motor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ford-motor, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ford-motor
provider_slug: ford-motor
slug: ford-motor-domain-security
source_filename: ford-motor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ford.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: api.ford.com\n  https: false\ndomains:\n- domain: ford.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ford-motor/refs/heads/main/security/ford-motor-domain-security.yml
summary_line: DMARC
tags:
- Fortune 100
---
