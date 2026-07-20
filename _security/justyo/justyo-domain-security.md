---
api_specs:
- filename: justyo-yo-openapi.yml
  format: yaml
  label: Yo API
  slug: yo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justyo/refs/heads/main/openapi/justyo-yo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: justyo.co
  spf: true
hosts:
- host: justyo.co
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Justyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for justyo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: justyo
provider_slug: justyo
slug: justyo-domain-security
source_filename: justyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justyo.co\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: justyo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justyo/refs/heads/main/security/justyo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Notifications
- Push Notifications
- Messaging
- Mobile
- Developer Tools
- API
---
