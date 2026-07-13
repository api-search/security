---
api_specs:
- filename: circlecis-openapi.yml
  format: yaml
  label: CircleCI REST API V2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: circleci.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: circleci.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circlecis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CircleCI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CircleCI
provider_slug: circlecis
slug: circlecis-domain-security
source_filename: circlecis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circleci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: circleci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/security/circlecis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Continuous Deployment
- Continuous Integration
- DevOps
- Pipelines
- Workflows
---
