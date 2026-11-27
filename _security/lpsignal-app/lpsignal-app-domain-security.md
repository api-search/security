---
api_specs:
- filename: lpsignal-app-account-api-openapi.yml
  format: yaml
  label: LPSignal Account API
  slug: lpsignal-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-account-api-openapi.yml
- filename: lpsignal-app-agents-api-openapi.yml
  format: yaml
  label: LPSignal Agents API
  slug: lpsignal-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-agents-api-openapi.yml
- filename: lpsignal-app-meta-api-openapi.yml
  format: yaml
  label: LPSignal Meta API
  slug: lpsignal-app-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-meta-api-openapi.yml
- filename: lpsignal-app-pools-api-openapi.yml
  format: yaml
  label: LPSignal Pools API
  slug: lpsignal-app-pools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-pools-api-openapi.yml
- filename: lpsignal-app-signals-api-openapi.yml
  format: yaml
  label: LPSignal Signals API
  slug: lpsignal-app-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-signals-api-openapi.yml
- filename: lpsignal-app-smart-lps-api-openapi.yml
  format: yaml
  label: LPSignal smart LPs API
  slug: lpsignal-app-smart-lps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-smart-lps-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lpsignal.app
  spf: true
hosts:
- cert_expires: Dec 29 07:07:31 2026 GMT
  host: lpsignal.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LPSignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LPSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LPSignal
provider_slug: lpsignal-app
slug: lpsignal-app-domain-security
source_filename: lpsignal-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lpsignal.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 07:07:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lpsignal.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lpsignal-app/security/lpsignal-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LP Signals
- Impermanent Loss
---
