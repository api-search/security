---
api_specs:
- filename: chartmogul-openapi.yml
  format: yaml
  label: ChartMogul REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-openapi.yml
- filename: chartmogul-asyncapi.yml
  format: yaml
  label: ChartMogul Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chartmogul.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: chartmogul.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 13:34:48 2026 GMT
  host: dev.chartmogul.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.chartmogul.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chartmogul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChartMogul, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ChartMogul
provider_slug: chartmogul
slug: chartmogul-domain-security
source_filename: chartmogul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chartmogul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.chartmogul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:34:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.chartmogul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: chartmogul.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/security/chartmogul-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscription Analytics
- SaaS Metrics
- Revenue Analytics
- MRR
- Churn
- Cohorts
- Billing
---
