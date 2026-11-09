---
api_specs:
- filename: cronjob-de-benachrichtigungen-api-openapi.yml
  format: yaml
  label: Cronjob.de Benachrichtigungen API
  slug: cronjob-de-benachrichtigungen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-benachrichtigungen-api-openapi.yml
- filename: cronjob-de-cronjobs-und-heartbeats-api-openapi.yml
  format: yaml
  label: Cronjob.de Cronjobs und Heartbeats API
  slug: cronjob-de-cronjobs-und-heartbeats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-cronjobs-und-heartbeats-api-openapi.yml
- filename: cronjob-de-server-berwachung-und-ssl-api-openapi.yml
  format: yaml
  label: Cronjob.de Serverüberwachung und SSL API
  slug: cronjob-de-server-berwachung-und-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-server-berwachung-und-ssl-api-openapi.yml
- filename: cronjob-de-statusseiten-api-openapi.yml
  format: yaml
  label: Cronjob.de Statusseiten API
  slug: cronjob-de-statusseiten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-statusseiten-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cronjob.de
  spf: true
hosts:
- cert_expires: Dec  6 07:18:12 2026 GMT
  host: cronjob.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cronjob De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cronjob.de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cronjob.de
provider_slug: cronjob-de
slug: cronjob-de-domain-security
source_filename: cronjob-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cronjob.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 07:18:12 2026 GMT\n  hsts: null\ndomains:\n- domain: cronjob.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cronjob-de/security/cronjob-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cronjob
- Scheduling
- Automation
- EU-hosted
---
