---
api_specs:
- filename: enzo-health-workflow-runs-api-openapi.yml
  format: yaml
  label: Enzo Health Workflow Runs API
  slug: enzo-health-workflow-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enzo-health/openapi/enzo-health-workflow-runs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enzo.health
  spf: true
hosts:
- cert_expires: Dec 10 18:06:21 2026 GMT
  host: www.enzo.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enzo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enzo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enzo Health
provider_slug: enzo-health
slug: enzo-health-domain-security
source_filename: enzo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enzo.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 18:06:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: enzo.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/enzo-health/security/enzo-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Home Health
- EHR
- Healthcare
- SaaS
---
