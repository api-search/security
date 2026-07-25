---
api_specs:
- filename: tableau-authentication-api-openapi.yml
  format: yaml
  label: Tableau Authentication API
  slug: tableau-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-authentication-api-openapi.yml
- filename: tableau-data-sources-api-openapi.yml
  format: yaml
  label: Tableau Data Sources API
  slug: tableau-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-data-sources-api-openapi.yml
- filename: tableau-favorites-api-openapi.yml
  format: yaml
  label: Tableau Favorites API
  slug: tableau-favorites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-favorites-api-openapi.yml
- filename: tableau-groups-api-openapi.yml
  format: yaml
  label: Tableau Groups API
  slug: tableau-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-groups-api-openapi.yml
- filename: tableau-jobs-api-openapi.yml
  format: yaml
  label: Tableau Jobs API
  slug: tableau-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-jobs-api-openapi.yml
- filename: tableau-permissions-api-openapi.yml
  format: yaml
  label: Tableau Permissions API
  slug: tableau-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-permissions-api-openapi.yml
- filename: tableau-projects-api-openapi.yml
  format: yaml
  label: Tableau Projects API
  slug: tableau-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-projects-api-openapi.yml
- filename: tableau-schedules-api-openapi.yml
  format: yaml
  label: Tableau Schedules API
  slug: tableau-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-schedules-api-openapi.yml
- filename: tableau-sites-api-openapi.yml
  format: yaml
  label: Tableau Sites API
  slug: tableau-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-sites-api-openapi.yml
- filename: tableau-subscriptions-api-openapi.yml
  format: yaml
  label: Tableau Subscriptions API
  slug: tableau-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-subscriptions-api-openapi.yml
- filename: tableau-users-api-openapi.yml
  format: yaml
  label: Tableau Users API
  slug: tableau-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-users-api-openapi.yml
- filename: tableau-views-api-openapi.yml
  format: yaml
  label: Tableau Views API
  slug: tableau-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-views-api-openapi.yml
- filename: tableau-workbooks-api-openapi.yml
  format: yaml
  label: Tableau Workbooks API
  slug: tableau-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-workbooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tableau.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: help.tableau.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tableau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tableau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tableau
provider_slug: tableau
slug: tableau-domain-security
source_filename: tableau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.tableau.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tableau.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/security/tableau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
---
