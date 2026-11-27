---
api_specs:
- filename: guarita-dev-apps-api-openapi.yml
  format: yaml
  label: Guarita Apps API
  slug: guarita-dev-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-apps-api-openapi.yml
- filename: guarita-dev-conta-api-openapi.yml
  format: yaml
  label: Guarita Conta API
  slug: guarita-dev-conta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-conta-api-openapi.yml
- filename: guarita-dev-relat-rio-api-openapi.yml
  format: yaml
  label: Guarita Relatório API
  slug: guarita-dev-relat-rio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-relat-rio-api-openapi.yml
- filename: guarita-dev-rondas-api-openapi.yml
  format: yaml
  label: Guarita Rondas API
  slug: guarita-dev-rondas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-rondas-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: guarita.dev
  spf: false
hosts:
- cert_expires: Jan 26 06:34:03 2027 GMT
  host: guarita.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Guarita Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guarita, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Guarita
provider_slug: guarita-dev
slug: guarita-dev-domain-security
source_filename: guarita-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guarita.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 06:34:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: guarita.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/guarita-dev/security/guarita-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
