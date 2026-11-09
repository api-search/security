---
api_specs:
- filename: botnotice-app-consent-api-openapi.yml
  format: yaml
  label: BotNotice Consent API
  slug: botnotice-app-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-consent-api-openapi.yml
- filename: botnotice-app-content-register-api-openapi.yml
  format: yaml
  label: BotNotice Content register API
  slug: botnotice-app-content-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-content-register-api-openapi.yml
- filename: botnotice-app-free-tools-api-openapi.yml
  format: yaml
  label: BotNotice Free tools API
  slug: botnotice-app-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-free-tools-api-openapi.yml
- filename: botnotice-app-law-dataset-api-openapi.yml
  format: yaml
  label: BotNotice Law dataset API
  slug: botnotice-app-law-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-law-dataset-api-openapi.yml
- filename: botnotice-app-voice-api-openapi.yml
  format: yaml
  label: BotNotice Voice API
  slug: botnotice-app-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-voice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botnotice.app
  spf: true
hosts:
- cert_expires: Dec  8 18:14:57 2026 GMT
  host: botnotice.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botnotice App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BotNotice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BotNotice
provider_slug: botnotice-app
slug: botnotice-app-domain-security
source_filename: botnotice-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botnotice.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 18:14:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: botnotice.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/botnotice-app/security/botnotice-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI disclosure
- chatbot compliance
- Recordkeeping
- website widget
- managed compliance
- subscription pricing
---
