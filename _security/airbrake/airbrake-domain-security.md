---
api_specs:
- filename: airbrake-openapi.yml
  format: yaml
  label: Airbrake API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@airbrake.io"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airbrake.io
  spf: true
hosts:
- cert_expires: Sep 14 05:18:46 2026 GMT
  host: www.airbrake.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: docs.airbrake.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.airbrake.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airbrake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbrake, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airbrake
provider_slug: airbrake
slug: airbrake-domain-security
source_filename: airbrake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airbrake.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:18:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.airbrake.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.airbrake.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: airbrake.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@airbrake.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/security/airbrake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Error Monitoring
- Application Performance Monitoring
- Observability
- DevOps
- Logging
- Exception Tracking
---
