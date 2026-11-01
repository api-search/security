---
api_specs:
- filename: flowmingo-flowmingo-api-api-openapi.yml
  format: yaml
  label: Flowmingo Flowmingo API
  slug: flowmingo-flowmingo-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowmingo/openapi/flowmingo-flowmingo-api-api-openapi.yml
- filename: flowmingo-scheduler-api-openapi.yml
  format: yaml
  label: Flowmingo Scheduler API
  slug: flowmingo-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowmingo/openapi/flowmingo-scheduler-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowmingo.ai
  spf: true
hosts:
- cert_expires: Oct 29 17:39:24 2026 GMT
  host: flowmingo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flowmingo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowmingo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flowmingo
provider_slug: flowmingo
slug: flowmingo-domain-security
source_filename: flowmingo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowmingo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:39:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowmingo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/flowmingo/security/flowmingo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
