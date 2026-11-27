---
api_specs:
- filename: piwik-pro-access-control-api-openapi.yml
  format: yaml
  label: Piwik PRO Access Control API
  slug: piwik-pro-access-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-access-control-api-openapi.yml
- filename: piwik-pro-analytics-api-openapi.yml
  format: yaml
  label: Piwik PRO Analytics API
  slug: piwik-pro-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-analytics-api-openapi.yml
- filename: piwik-pro-apps-api-openapi.yml
  format: yaml
  label: Piwik PRO Apps API
  slug: piwik-pro-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-apps-api-openapi.yml
- filename: piwik-pro-audit-log-api-openapi.yml
  format: yaml
  label: Piwik PRO Audit Log API
  slug: piwik-pro-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-audit-log-api-openapi.yml
- filename: piwik-pro-container-settings-api-openapi.yml
  format: yaml
  label: Piwik PRO Container Settings API
  slug: piwik-pro-container-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-container-settings-api-openapi.yml
- filename: piwik-pro-data-activation-api-openapi.yml
  format: yaml
  label: Piwik PRO Data Activation API
  slug: piwik-pro-data-activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-data-activation-api-openapi.yml
- filename: piwik-pro-meta-sites-api-openapi.yml
  format: yaml
  label: Piwik PRO Meta sites API
  slug: piwik-pro-meta-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-meta-sites-api-openapi.yml
- filename: piwik-pro-modules-api-openapi.yml
  format: yaml
  label: Piwik PRO Modules API
  slug: piwik-pro-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-modules-api-openapi.yml
- filename: piwik-pro-oauth-api-openapi.yml
  format: yaml
  label: Piwik PRO OAuth API
  slug: piwik-pro-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-oauth-api-openapi.yml
- filename: piwik-pro-tag-manager-api-openapi.yml
  format: yaml
  label: Piwik PRO Tag Manager API
  slug: piwik-pro-tag-manager-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tag-manager-api-openapi.yml
- filename: piwik-pro-tracker-api-openapi.yml
  format: yaml
  label: Piwik PRO Tracker API
  slug: piwik-pro-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tracker-api-openapi.yml
- filename: piwik-pro-tracker-settings-api-openapi.yml
  format: yaml
  label: Piwik PRO Tracker Settings API
  slug: piwik-pro-tracker-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tracker-settings-api-openapi.yml
- filename: piwik-pro-user-groups-api-openapi.yml
  format: yaml
  label: Piwik PRO User Groups API
  slug: piwik-pro-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-user-groups-api-openapi.yml
- filename: piwik-pro-users-api-openapi.yml
  format: yaml
  label: Piwik PRO Users API
  slug: piwik-pro-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: piwik.pro
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: piwik.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Piwik PRO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piwik PRO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Piwik PRO
provider_slug: piwik-pro
slug: piwik-pro-domain-security
source_filename: piwik-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: piwik.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: piwik.pro\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/piwik-pro/security/piwik-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Privacy
- Data Activation
- Enterprise
- Compliance
---
