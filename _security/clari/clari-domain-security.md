---
api_specs:
- filename: clari-copilot-api-openapi.yml
  format: yaml
  label: Clari Copilot API
  slug: clari-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-copilot-api-openapi.yml
- filename: clari-activity-api-api-openapi.yml
  format: yaml
  label: Clari Activity API API
  slug: clari-activity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-activity-api-api-openapi.yml
- filename: clari-administrative-api-api-openapi.yml
  format: yaml
  label: Clari Administrative API API
  slug: clari-administrative-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-administrative-api-api-openapi.yml
- filename: clari-audit-api-api-openapi.yml
  format: yaml
  label: Clari Audit API API
  slug: clari-audit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-audit-api-api-openapi.yml
- filename: clari-bulk-export-framework-api-openapi.yml
  format: yaml
  label: Clari Bulk Export Framework API
  slug: clari-bulk-export-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-export-framework-api-openapi.yml
- filename: clari-bulk-ingest-job-status-api-api-openapi.yml
  format: yaml
  label: Clari Bulk Ingest Job Status API API
  slug: clari-bulk-ingest-job-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-ingest-job-status-api-api-openapi.yml
- filename: clari-export-api-openapi.yml
  format: yaml
  label: Clari Export API
  slug: clari-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-export-api-openapi.yml
- filename: clari-forecast-api-api-openapi.yml
  format: yaml
  label: Clari Forecast API API
  slug: clari-forecast-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-forecast-api-api-openapi.yml
- filename: clari-ingestion-api-api-openapi.yml
  format: yaml
  label: Clari Ingestion API API
  slug: clari-ingestion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-ingestion-api-api-openapi.yml
- filename: clari-opportunity-api-api-openapi.yml
  format: yaml
  label: Clari Opportunity API API
  slug: clari-opportunity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-opportunity-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clari.com
  spf: true
hosts:
- cert_expires: Sep 19 16:41:18 2026 GMT
  host: www.clari.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api-doc.copilot.clari.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: rest-api.copilot.clari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clari, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clari
provider_slug: clari
slug: clari-domain-security
source_filename: clari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:41:18 2026 GMT\n  hsts: false\n- host: api-doc.copilot.clari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: rest-api.copilot.clari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: clari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/security/clari-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Revenue Operations
- Forecasting
- Pipeline Management
- Sales Intelligence
- Activity Intelligence
- Deal Insights
- CRM
- Conversation Intelligence
- B2B
- Enterprise
- MCP
- Agents
- Sales Engagement
- Bulk Export
- Data Ingestion
---
