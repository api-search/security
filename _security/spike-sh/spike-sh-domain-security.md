---
api_specs:
- filename: spike-sh-alert-rules-api-openapi.yml
  format: yaml
  label: Spike.sh Alert Rules API
  slug: spike-sh-alert-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-alert-rules-api-openapi.yml
- filename: spike-sh-components-api-openapi.yml
  format: yaml
  label: Spike.sh Components API
  slug: spike-sh-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-components-api-openapi.yml
- filename: spike-sh-escalations-api-openapi.yml
  format: yaml
  label: Spike.sh Escalations API
  slug: spike-sh-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-escalations-api-openapi.yml
- filename: spike-sh-incident-actions-api-openapi.yml
  format: yaml
  label: Spike.sh Incident Actions API
  slug: spike-sh-incident-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-incident-actions-api-openapi.yml
- filename: spike-sh-incidents-api-openapi.yml
  format: yaml
  label: Spike.sh Incidents API
  slug: spike-sh-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-incidents-api-openapi.yml
- filename: spike-sh-integrations-api-openapi.yml
  format: yaml
  label: Spike.sh Integrations API
  slug: spike-sh-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-integrations-api-openapi.yml
- filename: spike-sh-on-call-overrides-api-openapi.yml
  format: yaml
  label: Spike.sh On-Call Overrides API
  slug: spike-sh-on-call-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-on-call-overrides-api-openapi.yml
- filename: spike-sh-on-call-schedules-api-openapi.yml
  format: yaml
  label: Spike.sh On-Call Schedules API
  slug: spike-sh-on-call-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-on-call-schedules-api-openapi.yml
- filename: spike-sh-orgs-api-openapi.yml
  format: yaml
  label: Spike.sh Orgs API
  slug: spike-sh-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-orgs-api-openapi.yml
- filename: spike-sh-planned-maintenances-api-openapi.yml
  format: yaml
  label: Spike.sh Planned Maintenances API
  slug: spike-sh-planned-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-planned-maintenances-api-openapi.yml
- filename: spike-sh-services-api-openapi.yml
  format: yaml
  label: Spike.sh Services API
  slug: spike-sh-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-services-api-openapi.yml
- filename: spike-sh-status-page-incidents-api-openapi.yml
  format: yaml
  label: Spike.sh Status Page Incidents API
  slug: spike-sh-status-page-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-status-page-incidents-api-openapi.yml
- filename: spike-sh-status-pages-api-openapi.yml
  format: yaml
  label: Spike.sh Status Pages API
  slug: spike-sh-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-status-pages-api-openapi.yml
- filename: spike-sh-subscribers-api-openapi.yml
  format: yaml
  label: Spike.sh Subscribers API
  slug: spike-sh-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-subscribers-api-openapi.yml
- filename: spike-sh-suppressed-incidents-api-openapi.yml
  format: yaml
  label: Spike.sh Suppressed Incidents API
  slug: spike-sh-suppressed-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-suppressed-incidents-api-openapi.yml
- filename: spike-sh-teams-api-openapi.yml
  format: yaml
  label: Spike.sh Teams API
  slug: spike-sh-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-teams-api-openapi.yml
- filename: spike-sh-users-api-openapi.yml
  format: yaml
  label: Spike.sh Users API
  slug: spike-sh-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spike.sh
  spf: true
hosts:
- cert_expires: Aug 13 17:15:24 2026 GMT
  host: spike.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:08:56 2026 GMT
  host: docs.spike.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 12:51:24 2026 GMT
  host: api.spike.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spike Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spike.sh, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spike.sh
provider_slug: spike-sh
slug: spike-sh-domain-security
source_filename: spike-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spike.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spike.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:08:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spike.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spike.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/security/spike-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Incident Management
- On-Call
- Alerting
- Escalation Policies
- Status Pages
- Monitoring
- DevOps
- SRE
---
