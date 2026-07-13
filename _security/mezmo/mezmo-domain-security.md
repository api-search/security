---
api_specs:
- filename: mezmo-log-ingestion-api-openapi.yml
  format: yaml
  label: Mezmo Log Ingestion API
  slug: mezmo-log-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-log-ingestion-api-openapi.yml
- filename: mezmo-log-export-api-openapi.yml
  format: yaml
  label: Mezmo Log Export API
  slug: mezmo-log-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-log-export-api-openapi.yml
- filename: mezmo-views-api-openapi.yml
  format: yaml
  label: Mezmo Views API
  slug: mezmo-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-views-api-openapi.yml
- filename: mezmo-alerts-api-openapi.yml
  format: yaml
  label: Mezmo Alerts API
  slug: mezmo-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-alerts-api-openapi.yml
- filename: mezmo-archiving-api-openapi.yml
  format: yaml
  label: Mezmo Archiving API
  slug: mezmo-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-archiving-api-openapi.yml
- filename: mezmo-ingestion-control-api-openapi.yml
  format: yaml
  label: Mezmo Ingestion Control API
  slug: mezmo-ingestion-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-ingestion-control-api-openapi.yml
- filename: mezmo-usage-api-openapi.yml
  format: yaml
  label: Mezmo Usage API
  slug: mezmo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-usage-api-openapi.yml
- filename: mezmo-pipeline-api-openapi.yml
  format: yaml
  label: Mezmo Pipeline API
  slug: mezmo-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipeline-api-openapi.yml
- filename: mezmo-pipeline-classification-api-openapi.yml
  format: yaml
  label: Mezmo Pipeline Classification API
  slug: mezmo-pipeline-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipeline-classification-api-openapi.yml
- filename: mezmo-edge-api-openapi.yml
  format: yaml
  label: Mezmo Edge API
  slug: mezmo-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-edge-api-openapi.yml
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
- AI
- SRE
- OpenTelemetry
- DevOps
---
