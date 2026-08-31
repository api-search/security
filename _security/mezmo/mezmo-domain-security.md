---
api_specs:
- filename: mezmo-auditevents-api-openapi.yml
  format: yaml
  label: Mezmo AuditEvents API
  slug: mezmo-auditevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-auditevents-api-openapi.yml
- filename: mezmo-classification-api-openapi.yml
  format: yaml
  label: Mezmo Classification API
  slug: mezmo-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-classification-api-openapi.yml
- filename: mezmo-deployments-api-openapi.yml
  format: yaml
  label: Mezmo Deployments API
  slug: mezmo-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-deployments-api-openapi.yml
- filename: mezmo-destinations-api-openapi.yml
  format: yaml
  label: Mezmo Destinations API
  slug: mezmo-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-destinations-api-openapi.yml
- filename: mezmo-edgeclients-api-openapi.yml
  format: yaml
  label: Mezmo EdgeClients API
  slug: mezmo-edgeclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-edgeclients-api-openapi.yml
- filename: mezmo-exclusions-api-openapi.yml
  format: yaml
  label: Mezmo Exclusions API
  slug: mezmo-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-exclusions-api-openapi.yml
- filename: mezmo-export-api-openapi.yml
  format: yaml
  label: Mezmo Export API
  slug: mezmo-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-export-api-openapi.yml
- filename: mezmo-heartbeats-api-openapi.yml
  format: yaml
  label: Mezmo Heartbeats API
  slug: mezmo-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-heartbeats-api-openapi.yml
- filename: mezmo-logs-api-openapi.yml
  format: yaml
  label: Mezmo Logs API
  slug: mezmo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-logs-api-openapi.yml
- filename: mezmo-metrics-api-openapi.yml
  format: yaml
  label: Mezmo Metrics API
  slug: mezmo-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-metrics-api-openapi.yml
- filename: mezmo-pipelines-api-openapi.yml
  format: yaml
  label: Mezmo Pipelines API
  slug: mezmo-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipelines-api-openapi.yml
- filename: mezmo-presetalerts-api-openapi.yml
  format: yaml
  label: Mezmo PresetAlerts API
  slug: mezmo-presetalerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-presetalerts-api-openapi.yml
- filename: mezmo-processors-api-openapi.yml
  format: yaml
  label: Mezmo Processors API
  slug: mezmo-processors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-processors-api-openapi.yml
- filename: mezmo-sources-api-openapi.yml
  format: yaml
  label: Mezmo Sources API
  slug: mezmo-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-sources-api-openapi.yml
- filename: mezmo-suspension-api-openapi.yml
  format: yaml
  label: Mezmo Suspension API
  slug: mezmo-suspension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-suspension-api-openapi.yml
- filename: mezmo-tasks-api-openapi.yml
  format: yaml
  label: Mezmo Tasks API
  slug: mezmo-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mezmo.com
  spf: true
hosts:
- cert_expires: Oct  3 17:54:22 2026 GMT
  host: www.mezmo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:07:15 2026 GMT
  host: docs.mezmo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  7 08:52:20 2026 GMT
  host: api.mezmo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mezmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mezmo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mezmo
provider_slug: mezmo
slug: mezmo-domain-security
source_filename: mezmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mezmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:54:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mezmo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  1 07:07:15 2026 GMT\n  hsts: false\n- host: api.mezmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:52:20 2026 GMT\n  hsts: null\ndomains:\n- domain: mezmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/security/mezmo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Observability
- Logs
- Telemetry
- Telemetry Pipeline
- Log Management
- Artificial Intelligence
- SRE
- OpenTelemetry
- DevOps
---
