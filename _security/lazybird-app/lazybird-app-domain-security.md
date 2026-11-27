---
api_specs:
- filename: lazybird-app-auth-api-openapi.yml
  format: yaml
  label: Lazybird Auth API
  slug: lazybird-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-auth-api-openapi.yml
- filename: lazybird-app-checkout-api-openapi.yml
  format: yaml
  label: Lazybird Checkout API
  slug: lazybird-app-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-checkout-api-openapi.yml
- filename: lazybird-app-generate-speech-api-openapi.yml
  format: yaml
  label: Lazybird Generate Speech API
  slug: lazybird-app-generate-speech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-generate-speech-api-openapi.yml
- filename: lazybird-app-me-api-openapi.yml
  format: yaml
  label: Lazybird Me API
  slug: lazybird-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-me-api-openapi.yml
- filename: lazybird-app-music-api-openapi.yml
  format: yaml
  label: Lazybird Music API
  slug: lazybird-app-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-music-api-openapi.yml
- filename: lazybird-app-projects-api-openapi.yml
  format: yaml
  label: Lazybird Projects API
  slug: lazybird-app-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-projects-api-openapi.yml
- filename: lazybird-app-status-api-openapi.yml
  format: yaml
  label: Lazybird Status API
  slug: lazybird-app-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-status-api-openapi.yml
- filename: lazybird-app-stock-api-openapi.yml
  format: yaml
  label: Lazybird Stock API
  slug: lazybird-app-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-stock-api-openapi.yml
- filename: lazybird-app-voices-api-openapi.yml
  format: yaml
  label: Lazybird Voices API
  slug: lazybird-app-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lazybird.app
  spf: true
hosts:
- cert_expires: Dec 23 20:27:10 2026 GMT
  host: www.lazybird.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 05:10:50 2027 GMT
  host: api.lazybird.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Lazybird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lazybird, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lazybird
provider_slug: lazybird-app
slug: lazybird-app-domain-security
source_filename: lazybird-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lazybird.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lazybird.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:10:50 2027 GMT\n  hsts: false\ndomains:\n- domain: lazybird.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lazybird-app/security/lazybird-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Voiceover
- Text-to-Speech
- Creator Tools
- Multilingual
---
