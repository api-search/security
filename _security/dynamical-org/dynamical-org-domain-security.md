---
api_specs:
- filename: dynamical-org-analyses-api-openapi.yml
  format: yaml
  label: Dynamical Analyses API
  slug: dynamical-org-analyses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-analyses-api-openapi.yml
- filename: dynamical-org-data-api-openapi.yml
  format: yaml
  label: Dynamical Data API
  slug: dynamical-org-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-data-api-openapi.yml
- filename: dynamical-org-data-products-api-openapi.yml
  format: yaml
  label: Dynamical Data Products API
  slug: dynamical-org-data-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-data-products-api-openapi.yml
- filename: dynamical-org-forecasts-api-openapi.yml
  format: yaml
  label: Dynamical Forecasts API
  slug: dynamical-org-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-forecasts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dynamical.org
  spf: true
hosts:
- cert_expires: Jan 14 15:44:26 2027 GMT
  host: dynamical.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynamical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dynamical
provider_slug: dynamical-org
slug: dynamical-org-domain-security
source_filename: dynamical-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynamical.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:44:26 2027 GMT\n  hsts: false\ndomains:\n- domain: dynamical.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dynamical-org/security/dynamical-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Climate
- Open Data
- Research
- Not-for-profit
---
