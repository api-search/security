---
api_specs:
- filename: opensensors-analytics-api-openapi.yml
  format: yaml
  label: OpenSensors Analytics API
  slug: opensensors-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opensensors/openapi/opensensors-analytics-api-openapi.yml
- filename: opensensors-authentication-api-openapi.yml
  format: yaml
  label: OpenSensors Authentication API
  slug: opensensors-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opensensors/openapi/opensensors-authentication-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opensensors.com
  spf: true
hosts:
- cert_expires: Dec  9 18:24:42 2026 GMT
  host: opensensors.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opensensors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSensors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenSensors
provider_slug: opensensors
slug: opensensors-domain-security
source_filename: opensensors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensensors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 18:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opensensors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/opensensors/security/opensensors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- WorkplaceAnalytics
- RealEstateTech
- IoT
- DataAnalytics
---
