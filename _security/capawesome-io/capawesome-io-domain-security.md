---
api_specs:
- filename: capawesome-io-app-build-shares-api-openapi.yml
  format: yaml
  label: capawesome-io App Build Shares API
  slug: capawesome-io-app-build-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capawesome-io/openapi/capawesome-io-app-build-shares-api-openapi.yml
- filename: capawesome-io-apps-api-openapi.yml
  format: yaml
  label: capawesome-io Apps API
  slug: capawesome-io-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capawesome-io/openapi/capawesome-io-apps-api-openapi.yml
- filename: capawesome-io-jobs-api-openapi.yml
  format: yaml
  label: capawesome-io Jobs API
  slug: capawesome-io-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capawesome-io/openapi/capawesome-io-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capawesome.io
  spf: true
hosts:
- cert_expires: Jan 20 16:01:17 2027 GMT
  host: capawesome.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capawesome Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for capawesome-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: capawesome-io
provider_slug: capawesome-io
slug: capawesome-io-domain-security
source_filename: capawesome-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capawesome.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 16:01:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capawesome.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/capawesome-io/security/capawesome-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile
- DevOps
- CI/CD
- OTA
- Capacitor
- Ionic
---
