---
api_specs:
- filename: fingoal-insights-openapi-original.json
  format: json
  label: FinGoal Insights API
  slug: fingoal-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-insights-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fingoal.com
  spf: true
hosts:
- cert_expires: Aug  9 21:12:05 2026 GMT
  host: fingoal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:51:33 2026 GMT
  host: findmoney-dev.fingoal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:51:33 2026 GMT
  host: findmoney.fingoal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fingoal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinGoal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FinGoal
provider_slug: fingoal
slug: fingoal-domain-security
source_filename: fingoal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fingoal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 21:12:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: findmoney-dev.fingoal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:51:33 2026 GMT\n  hsts: null\n- host: findmoney.fingoal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:51:33 2026 GMT\n  hsts: null\ndomains:\n- domain: fingoal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/security/fingoal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Fintech
- Transaction Enrichment
- Data Enrichment
- Personal Financial Management
- Banking
- Categorization
- Webhooks
---
