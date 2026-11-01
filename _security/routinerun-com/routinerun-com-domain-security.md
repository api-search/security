---
api_specs:
- filename: routinerun-com-events-api-openapi.yml
  format: yaml
  label: routinerun-com Events API
  slug: routinerun-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-events-api-openapi.yml
- filename: routinerun-com-runs-api-openapi.yml
  format: yaml
  label: routinerun-com Runs API
  slug: routinerun-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-runs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: routinerun.com
  spf: true
hosts:
- cert_expires: Dec 14 17:48:03 2026 GMT
  host: routinerun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Routinerun Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for routinerun-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: routinerun-com
provider_slug: routinerun-com
slug: routinerun-com-domain-security
source_filename: routinerun-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routinerun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 17:48:03 2026 GMT\n  hsts: false\ndomains:\n- domain: routinerun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/routinerun-com/security/routinerun-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automation
- Productivity
- Task Management
- No-code
---
