---
api_specs:
- filename: reflecto-dev-devices-api-openapi.yml
  format: yaml
  label: Reflecto Devices API
  slug: reflecto-dev-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-devices-api-openapi.yml
- filename: reflecto-dev-interactions-api-openapi.yml
  format: yaml
  label: Reflecto Interactions API
  slug: reflecto-dev-interactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-interactions-api-openapi.yml
- filename: reflecto-dev-pushover-compatibility-api-openapi.yml
  format: yaml
  label: Reflecto Pushover compatibility API
  slug: reflecto-dev-pushover-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-pushover-compatibility-api-openapi.yml
- filename: reflecto-dev-reminders-api-openapi.yml
  format: yaml
  label: Reflecto Reminders API
  slug: reflecto-dev-reminders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-reminders-api-openapi.yml
- filename: reflecto-dev-send-api-openapi.yml
  format: yaml
  label: Reflecto Send API
  slug: reflecto-dev-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-send-api-openapi.yml
- filename: reflecto-dev-sms-assistant-api-openapi.yml
  format: yaml
  label: Reflecto SMS (assistant) API
  slug: reflecto-dev-sms-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-sms-assistant-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reflecto.dev
  spf: true
hosts:
- cert_expires: Jan  5 13:07:55 2027 GMT
  host: reflecto.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reflecto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reflecto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Reflecto
provider_slug: reflecto-dev
slug: reflecto-dev-domain-security
source_filename: reflecto-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reflecto.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:07:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reflecto.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reflecto-dev/security/reflecto-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Notification
- Encryption
- Cross-Device
- Open-Source
---
