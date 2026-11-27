---
api_specs:
- filename: logbrew-account-api-openapi.yml
  format: yaml
  label: LogBrew Account API
  slug: logbrew-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-account-api-openapi.yml
- filename: logbrew-actions-api-openapi.yml
  format: yaml
  label: LogBrew Actions API
  slug: logbrew-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-actions-api-openapi.yml
- filename: logbrew-alerts-api-openapi.yml
  format: yaml
  label: LogBrew Alerts API
  slug: logbrew-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-alerts-api-openapi.yml
- filename: logbrew-billing-api-openapi.yml
  format: yaml
  label: LogBrew Billing API
  slug: logbrew-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-billing-api-openapi.yml
- filename: logbrew-connected-clients-api-openapi.yml
  format: yaml
  label: LogBrew Connected clients API
  slug: logbrew-connected-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-connected-clients-api-openapi.yml
- filename: logbrew-debug-files-api-openapi.yml
  format: yaml
  label: LogBrew Debug files API
  slug: logbrew-debug-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-debug-files-api-openapi.yml
- filename: logbrew-ingestion-api-openapi.yml
  format: yaml
  label: LogBrew Ingestion API
  slug: logbrew-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-ingestion-api-openapi.yml
- filename: logbrew-issues-api-openapi.yml
  format: yaml
  label: LogBrew Issues API
  slug: logbrew-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-issues-api-openapi.yml
- filename: logbrew-live-feed-api-openapi.yml
  format: yaml
  label: LogBrew Live feed API
  slug: logbrew-live-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-live-feed-api-openapi.yml
- filename: logbrew-logs-api-openapi.yml
  format: yaml
  label: LogBrew Logs API
  slug: logbrew-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-logs-api-openapi.yml
- filename: logbrew-metrics-api-openapi.yml
  format: yaml
  label: LogBrew Metrics API
  slug: logbrew-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-metrics-api-openapi.yml
- filename: logbrew-organizations-api-openapi.yml
  format: yaml
  label: LogBrew Organizations API
  slug: logbrew-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-organizations-api-openapi.yml
- filename: logbrew-product-analytics-api-openapi.yml
  format: yaml
  label: LogBrew Product analytics API
  slug: logbrew-product-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-product-analytics-api-openapi.yml
- filename: logbrew-projects-api-openapi.yml
  format: yaml
  label: LogBrew Projects API
  slug: logbrew-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-projects-api-openapi.yml
- filename: logbrew-releases-api-openapi.yml
  format: yaml
  label: LogBrew Releases API
  slug: logbrew-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-releases-api-openapi.yml
- filename: logbrew-support-api-openapi.yml
  format: yaml
  label: LogBrew Support API
  slug: logbrew-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-support-api-openapi.yml
- filename: logbrew-traces-api-openapi.yml
  format: yaml
  label: LogBrew Traces API
  slug: logbrew-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-traces-api-openapi.yml
- filename: logbrew-volume-api-openapi.yml
  format: yaml
  label: LogBrew Volume API
  slug: logbrew-volume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-volume-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@logbrew.co"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: logbrew.co
  spf: true
hosts:
- cert_expires: Jan 23 14:59:23 2027 GMT
  host: logbrew.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LogBrew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LogBrew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LogBrew
provider_slug: logbrew
slug: logbrew-domain-security
source_filename: logbrew-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logbrew.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:59:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: logbrew.co\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@logbrew.co\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/logbrew/security/logbrew-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Observability
- Logging
- Monitoring
- Analytics
- Error Tracking
---
