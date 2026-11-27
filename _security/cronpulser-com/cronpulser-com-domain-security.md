---
api_specs:
- filename: cronpulser-com-openapi-generated.yml
  format: yaml
  label: CronPulser API
  slug: cronpulser-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronpulser-com/openapi/_ae-authored/cronpulser-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cronpulser.com
  spf: true
hosts:
- cert_expires: Jan 31 18:57:26 2027 GMT
  host: cronpulser.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CronPulser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CronPulser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CronPulser
provider_slug: cronpulser-com
slug: cronpulser-com-domain-security
source_filename: cronpulser-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cronpulser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 18:57:26 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cronpulser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cronpulser-com/security/cronpulser-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HTTP Scheduler
- API Scheduling
- Runner
- TLS Monitoring
---
