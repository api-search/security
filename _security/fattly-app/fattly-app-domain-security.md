---
api_specs:
- filename: fattly-app-account-api-openapi.yml
  format: yaml
  label: Fattly AI Account API
  slug: fattly-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-account-api-openapi.yml
- filename: fattly-app-ad-studio-api-openapi.yml
  format: yaml
  label: Fattly AI Ad Studio API
  slug: fattly-app-ad-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-ad-studio-api-openapi.yml
- filename: fattly-app-audio-api-openapi.yml
  format: yaml
  label: Fattly AI Audio API
  slug: fattly-app-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-audio-api-openapi.yml
- filename: fattly-app-images-api-openapi.yml
  format: yaml
  label: Fattly AI Images API
  slug: fattly-app-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-images-api-openapi.yml
- filename: fattly-app-video-api-openapi.yml
  format: yaml
  label: Fattly AI Video API
  slug: fattly-app-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-video-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fattly.app
  spf: true
hosts:
- cert_expires: Jan 24 16:43:52 2027 GMT
  host: fattly.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fattly App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fattly AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fattly AI
provider_slug: fattly-app
slug: fattly-app-domain-security
source_filename: fattly-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fattly.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 16:43:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fattly.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fattly-app/security/fattly-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Image Generation
- Video Generation
- Marketing
- Content Creation
---
