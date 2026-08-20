---
api_specs:
- filename: opsgenie-account-api-openapi.yml
  format: yaml
  label: OpsGenie Account API
  slug: opsgenie-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-account-api-openapi.yml
- filename: opsgenie-alerts-api-openapi.yml
  format: yaml
  label: OpsGenie Alerts API
  slug: opsgenie-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-alerts-api-openapi.yml
- filename: opsgenie-escalations-api-openapi.yml
  format: yaml
  label: OpsGenie Escalations API
  slug: opsgenie-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-escalations-api-openapi.yml
- filename: opsgenie-heartbeats-api-openapi.yml
  format: yaml
  label: OpsGenie Heartbeats API
  slug: opsgenie-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-heartbeats-api-openapi.yml
- filename: opsgenie-incidents-api-openapi.yml
  format: yaml
  label: OpsGenie Incidents API
  slug: opsgenie-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-incidents-api-openapi.yml
- filename: opsgenie-integrations-api-openapi.yml
  format: yaml
  label: OpsGenie Integrations API
  slug: opsgenie-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-integrations-api-openapi.yml
- filename: opsgenie-maintenance-api-openapi.yml
  format: yaml
  label: OpsGenie Maintenance API
  slug: opsgenie-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-maintenance-api-openapi.yml
- filename: opsgenie-notification-rules-api-openapi.yml
  format: yaml
  label: OpsGenie Notification Rules API
  slug: opsgenie-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-notification-rules-api-openapi.yml
- filename: opsgenie-on-call-api-openapi.yml
  format: yaml
  label: OpsGenie On-Call API
  slug: opsgenie-on-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-on-call-api-openapi.yml
- filename: opsgenie-overrides-api-openapi.yml
  format: yaml
  label: OpsGenie Overrides API
  slug: opsgenie-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-overrides-api-openapi.yml
- filename: opsgenie-rotations-api-openapi.yml
  format: yaml
  label: OpsGenie Rotations API
  slug: opsgenie-rotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-rotations-api-openapi.yml
- filename: opsgenie-schedules-api-openapi.yml
  format: yaml
  label: OpsGenie Schedules API
  slug: opsgenie-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-schedules-api-openapi.yml
- filename: opsgenie-services-api-openapi.yml
  format: yaml
  label: OpsGenie Services API
  slug: opsgenie-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-services-api-openapi.yml
- filename: opsgenie-teams-api-openapi.yml
  format: yaml
  label: OpsGenie Teams API
  slug: opsgenie-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-teams-api-openapi.yml
- filename: opsgenie-users-api-openapi.yml
  format: yaml
  label: OpsGenie Users API
  slug: opsgenie-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opsgenie.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atlassian.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: docs.opsgenie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.opsgenie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opsgenie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpsGenie, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpsGenie
provider_slug: opsgenie
slug: opsgenie-domain-security
source_filename: opsgenie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.opsgenie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: www.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.opsgenie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: opsgenie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: atlassian.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/security/opsgenie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Alerts
- Incident Management
- Monitoring
- On-Call
---
