---
api_specs:
- filename: opsgenie-alert-openapi.yml
  format: yaml
  label: OpsGenie Alert API
  slug: opsgenie-alert
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-alert-openapi.yml
- filename: opsgenie-incident-openapi.yml
  format: yaml
  label: OpsGenie Incident API
  slug: opsgenie-incident
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-incident-openapi.yml
- filename: opsgenie-user-openapi.yml
  format: yaml
  label: OpsGenie User API
  slug: opsgenie-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-user-openapi.yml
- filename: opsgenie-team-openapi.yml
  format: yaml
  label: OpsGenie Team API
  slug: opsgenie-team
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-team-openapi.yml
- filename: opsgenie-schedule-openapi.yml
  format: yaml
  label: OpsGenie Schedule API
  slug: opsgenie-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-schedule-openapi.yml
- filename: opsgenie-escalation-openapi.yml
  format: yaml
  label: OpsGenie Escalation API
  slug: opsgenie-escalation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-escalation-openapi.yml
- filename: opsgenie-integration-openapi.yml
  format: yaml
  label: OpsGenie Integration API
  slug: opsgenie-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-integration-openapi.yml
- filename: opsgenie-heartbeat-openapi.yml
  format: yaml
  label: OpsGenie Heartbeat API
  slug: opsgenie-heartbeat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-heartbeat-openapi.yml
- filename: opsgenie-service-openapi.yml
  format: yaml
  label: OpsGenie Service API
  slug: opsgenie-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-service-openapi.yml
- filename: opsgenie-notification-rule-openapi.yml
  format: yaml
  label: OpsGenie Notification Rule API
  slug: opsgenie-notification-rule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-notification-rule-openapi.yml
- filename: opsgenie-account-openapi.yml
  format: yaml
  label: OpsGenie Account API
  slug: opsgenie-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-account-openapi.yml
- filename: opsgenie-maintenance-openapi.yml
  format: yaml
  label: OpsGenie Maintenance API
  slug: opsgenie-maintenance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-maintenance-openapi.yml
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
- Operations
---
