---
api_specs:
- filename: infivoice-agents-api-openapi.yml
  format: yaml
  label: InfiVoice Agents API
  slug: infivoice-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-agents-api-openapi.yml
- filename: infivoice-analytics-api-openapi.yml
  format: yaml
  label: InfiVoice Analytics API
  slug: infivoice-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-analytics-api-openapi.yml
- filename: infivoice-calls-api-openapi.yml
  format: yaml
  label: InfiVoice Calls API
  slug: infivoice-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-calls-api-openapi.yml
- filename: infivoice-campaigns-api-openapi.yml
  format: yaml
  label: InfiVoice Campaigns API
  slug: infivoice-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-campaigns-api-openapi.yml
- filename: infivoice-contacts-api-openapi.yml
  format: yaml
  label: InfiVoice Contacts API
  slug: infivoice-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-contacts-api-openapi.yml
- filename: infivoice-credits-api-openapi.yml
  format: yaml
  label: InfiVoice Credits API
  slug: infivoice-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-credits-api-openapi.yml
- filename: infivoice-introduction-api-openapi.yml
  format: yaml
  label: InfiVoice Introduction API
  slug: infivoice-introduction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-introduction-api-openapi.yml
- filename: infivoice-webhooks-api-openapi.yml
  format: yaml
  label: InfiVoice Webhooks API
  slug: infivoice-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infivoice.com
  spf: true
hosts:
- cert_expires: Jan 15 05:50:19 2027 GMT
  host: infivoice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InfiVoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InfiVoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InfiVoice
provider_slug: infivoice
slug: infivoice-domain-security
source_filename: infivoice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infivoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 05:50:19 2027 GMT\n  hsts: false\ndomains:\n- domain: infivoice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/infivoice/security/infivoice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Voice
- Automation
- Software-as-a-Service
---
