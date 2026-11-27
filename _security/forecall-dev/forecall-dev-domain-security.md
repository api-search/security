---
api_specs:
- filename: forecall-dev-evaluations-api-openapi.yml
  format: yaml
  label: forecall-dev Evaluations API
  slug: forecall-dev-evaluations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecall-dev/openapi/forecall-dev-evaluations-api-openapi.yml
- filename: forecall-dev-me-api-openapi.yml
  format: yaml
  label: forecall-dev Me API
  slug: forecall-dev-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecall-dev/openapi/forecall-dev-me-api-openapi.yml
- filename: forecall-dev-servers-api-openapi.yml
  format: yaml
  label: forecall-dev Servers API
  slug: forecall-dev-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecall-dev/openapi/forecall-dev-servers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forecall.dev
  spf: true
hosts:
- cert_expires: Jan  5 10:11:06 2027 GMT
  host: forecall.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: forecall-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for forecall-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: forecall-dev
provider_slug: forecall-dev
slug: forecall-dev-domain-security
source_filename: forecall-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forecall.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 10:11:06 2027 GMT\n  hsts: false\ndomains:\n- domain: forecall.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/forecall-dev/security/forecall-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Static Linter
- Description Scoring
- Failure Records
---
