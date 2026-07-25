---
api_specs:
- filename: quasar-cluster-api-openapi.yml
  format: yaml
  label: Quasar cluster API
  slug: quasar-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-cluster-api-openapi.yml
- filename: quasar-login-api-openapi.yml
  format: yaml
  label: Quasar Login API
  slug: quasar-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-login-api-openapi.yml
- filename: quasar-max-in-buffer-size-api-openapi.yml
  format: yaml
  label: Quasar max-in-buffer-size API
  slug: quasar-max-in-buffer-size-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-max-in-buffer-size-api-openapi.yml
- filename: quasar-option-api-openapi.yml
  format: yaml
  label: Quasar option API
  slug: quasar-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-option-api-openapi.yml
- filename: quasar-parallelism-api-openapi.yml
  format: yaml
  label: Quasar parallelism API
  slug: quasar-parallelism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-parallelism-api-openapi.yml
- filename: quasar-prometheus-api-openapi.yml
  format: yaml
  label: Quasar Prometheus API
  slug: quasar-prometheus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-prometheus-api-openapi.yml
- filename: quasar-query-api-openapi.yml
  format: yaml
  label: Quasar query API
  slug: quasar-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-query-api-openapi.yml
- filename: quasar-status-api-openapi.yml
  format: yaml
  label: Quasar Status API
  slug: quasar-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-status-api-openapi.yml
- filename: quasar-tables-api-openapi.yml
  format: yaml
  label: Quasar Tables API
  slug: quasar-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-tables-api-openapi.yml
- filename: quasar-tags-api-openapi.yml
  format: yaml
  label: Quasar tags API
  slug: quasar-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-tags-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: quasar.ai
  spf: true
hosts:
- cert_expires: Aug 30 20:35:26 2026 GMT
  host: quasar.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quasar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quasar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Quasar
provider_slug: quasar
slug: quasar-domain-security
source_filename: quasar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quasar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 20:35:26 2026 GMT\n  hsts: false\ndomains:\n- domain: quasar.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/security/quasar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Time Series Database
- Database
- Analytics
- Infrastructure
- Real-Time Data
- Aerospace
- Finance
---
