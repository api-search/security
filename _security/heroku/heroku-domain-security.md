---
api_specs:
- filename: heroku-platform-api.yml
  format: yaml
  label: Heroku Platform API
  slug: heroku-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-platform-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heroku.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: devcenter.heroku.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 07:02:04 2026 GMT
  host: www.heroku.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.heroku.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heroku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heroku, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heroku
provider_slug: heroku
slug: heroku-domain-security
source_filename: heroku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devcenter.heroku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.heroku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 07:02:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.heroku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: heroku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/security/heroku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Deployment
- Cloud Platform
- DevOps
- PaaS
---
