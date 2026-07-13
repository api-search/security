---
api_specs:
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Providers API
  slug: providers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Services API
  slug: services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: spurwing.io
  spf: true
hosts:
- host: www.spurwing.io
  https: false
- host: docs.spurwing.io
  https: false
- host: api.spurwing.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Spurwing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spurwing, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spurwing
provider_slug: spurwing
slug: spurwing-domain-security
source_filename: spurwing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spurwing.io\n  https: false\n- host: docs.spurwing.io\n  https: false\n- host: api.spurwing.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: spurwing.io\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/security/spurwing-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Scheduling
- Appointments
- Booking
- Calendar
- Availability
---
