---
api_specs:
- filename: mida-so-account-api-openapi.yml
  format: yaml
  label: Mida Account API
  slug: mida-so-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-account-api-openapi.yml
- filename: mida-so-events-api-openapi.yml
  format: yaml
  label: Mida Events API
  slug: mida-so-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-events-api-openapi.yml
- filename: mida-so-exclusion-groups-api-openapi.yml
  format: yaml
  label: Mida Exclusion groups API
  slug: mida-so-exclusion-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-exclusion-groups-api-openapi.yml
- filename: mida-so-experiments-api-openapi.yml
  format: yaml
  label: Mida Experiments API
  slug: mida-so-experiments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-experiments-api-openapi.yml
- filename: mida-so-goals-api-openapi.yml
  format: yaml
  label: Mida Goals API
  slug: mida-so-goals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-goals-api-openapi.yml
- filename: mida-so-hypotheses-api-openapi.yml
  format: yaml
  label: Mida Hypotheses API
  slug: mida-so-hypotheses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-hypotheses-api-openapi.yml
- filename: mida-so-personalization-api-openapi.yml
  format: yaml
  label: Mida Personalization API
  slug: mida-so-personalization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-personalization-api-openapi.yml
- filename: mida-so-projects-api-openapi.yml
  format: yaml
  label: Mida Projects API
  slug: mida-so-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-projects-api-openapi.yml
- filename: mida-so-surveys-api-openapi.yml
  format: yaml
  label: Mida Surveys API
  slug: mida-so-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-surveys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mida.so
  spf: true
hosts:
- cert_expires: Feb  9 16:56:03 2027 GMT
  host: mida.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mida Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mida, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mida
provider_slug: mida-so
slug: mida-so-domain-security
source_filename: mida-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mida.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 16:56:03 2027 GMT\n  hsts: false\ndomains:\n- domain: mida.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mida-so/security/mida-so-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- A/B Testing
- Artificial Intelligence
- Marketing
- Analytics
- Software-as-a-Service
- Platform
---
