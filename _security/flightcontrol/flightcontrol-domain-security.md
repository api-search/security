---
api_specs:
- filename: flightcontrol-openapi.yml
  format: yaml
  label: Flightcontrol Management API
  slug: flightcontrol-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-openapi.yml
- filename: flightcontrol-openapi.yml
  format: yaml
  label: Flightcontrol Deploy Hooks API
  slug: flightcontrol-deploy-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-openapi.yml
- filename: flightcontrol-openapi.yml
  format: yaml
  label: Flightcontrol CloudFront Invalidation API
  slug: flightcontrol-cloudfront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flightcontrol.dev
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.flightcontrol.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.flightcontrol.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: app.flightcontrol.dev
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flightcontrol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flightcontrol, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flightcontrol
provider_slug: flightcontrol
slug: flightcontrol-domain-security
source_filename: flightcontrol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flightcontrol.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flightcontrol.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\n- host: app.flightcontrol.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: flightcontrol.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/security/flightcontrol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Deployment
- PaaS
- Infrastructure
- DevOps
---
