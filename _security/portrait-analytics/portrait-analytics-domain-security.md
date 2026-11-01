---
api_specs:
- filename: portrait-analytics-openapi-generated.yml
  format: yaml
  label: Portrait Analytics API
  slug: portrait-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/portrait-analytics/openapi/_ae-authored/portrait-analytics-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: portraitresearch.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: portraitresearch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Portrait Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portrait Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Portrait Analytics
provider_slug: portrait-analytics
slug: portrait-analytics-domain-security
source_filename: portrait-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portraitresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: portraitresearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/portrait-analytics/security/portrait-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Finance
- Research
- Investment
- Data
---
