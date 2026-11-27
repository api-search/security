---
api_specs:
- filename: openuptime-app-openapi-generated.yml
  format: yaml
  label: OpenUptime API
  slug: openuptime-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openuptime-app/openapi/_ae-authored/openuptime-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openuptime.app
  spf: true
hosts:
- cert_expires: Jan  8 17:58:33 2027 GMT
  host: openuptime.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenUptime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenUptime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenUptime
provider_slug: openuptime-app
slug: openuptime-app-domain-security
source_filename: openuptime-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openuptime.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:58:33 2027 GMT\n  hsts: false\ndomains:\n- domain: openuptime.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openuptime-app/security/openuptime-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Monitoring
- Open Source
- Status Pages
- Alerts
- Uptime
---
