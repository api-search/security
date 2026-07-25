---
api_specs:
- filename: checkly-accounts-api-openapi.yml
  format: yaml
  label: Checkly Accounts API
  slug: checkly-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-accounts-api-openapi.yml
- filename: checkly-alert-channels-api-openapi.yml
  format: yaml
  label: Checkly Alert Channels API
  slug: checkly-alert-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-alert-channels-api-openapi.yml
- filename: checkly-analytics-api-openapi.yml
  format: yaml
  label: Checkly Analytics API
  slug: checkly-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-analytics-api-openapi.yml
- filename: checkly-check-alerts-api-openapi.yml
  format: yaml
  label: Checkly Check Alerts API
  slug: checkly-check-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-alerts-api-openapi.yml
- filename: checkly-check-groups-api-openapi.yml
  format: yaml
  label: Checkly Check Groups API
  slug: checkly-check-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-groups-api-openapi.yml
- filename: checkly-check-results-api-openapi.yml
  format: yaml
  label: Checkly Check Results API
  slug: checkly-check-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-results-api-openapi.yml
- filename: checkly-check-statuses-api-openapi.yml
  format: yaml
  label: Checkly Check Statuses API
  slug: checkly-check-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-statuses-api-openapi.yml
- filename: checkly-checks-api-openapi.yml
  format: yaml
  label: Checkly Checks API
  slug: checkly-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-checks-api-openapi.yml
- filename: checkly-dashboards-api-openapi.yml
  format: yaml
  label: Checkly Dashboards API
  slug: checkly-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-dashboards-api-openapi.yml
- filename: checkly-heartbeats-api-openapi.yml
  format: yaml
  label: Checkly Heartbeats API
  slug: checkly-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-heartbeats-api-openapi.yml
- filename: checkly-incidents-api-openapi.yml
  format: yaml
  label: Checkly Incidents API
  slug: checkly-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-incidents-api-openapi.yml
- filename: checkly-locations-api-openapi.yml
  format: yaml
  label: Checkly Locations API
  slug: checkly-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-locations-api-openapi.yml
- filename: checkly-maintenance-windows-api-openapi.yml
  format: yaml
  label: Checkly Maintenance Windows API
  slug: checkly-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-maintenance-windows-api-openapi.yml
- filename: checkly-private-locations-api-openapi.yml
  format: yaml
  label: Checkly Private Locations API
  slug: checkly-private-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-private-locations-api-openapi.yml
- filename: checkly-reports-api-openapi.yml
  format: yaml
  label: Checkly Reports API
  slug: checkly-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-reports-api-openapi.yml
- filename: checkly-variables-api-openapi.yml
  format: yaml
  label: Checkly Variables API
  slug: checkly-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-variables-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: checklyhq.com
  spf: true
hosts:
- cert_expires: Oct  7 23:32:51 2026 GMT
  host: www.checklyhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 00:34:53 2026 GMT
  host: api.checklyhq.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Checkly
provider_slug: checkly
slug: checkly-domain-security
source_filename: checkly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checklyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:32:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.checklyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:34:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: checklyhq.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/security/checkly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Testing
---
