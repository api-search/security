---
api_specs:
- filename: sifflet-assets-api-openapi.yml
  format: yaml
  label: Sifflet Assets API
  slug: sifflet-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-assets-api-openapi.yml
- filename: sifflet-calendars-api-openapi.yml
  format: yaml
  label: Sifflet Calendars API
  slug: sifflet-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-calendars-api-openapi.yml
- filename: sifflet-credentials-api-openapi.yml
  format: yaml
  label: Sifflet Credentials API
  slug: sifflet-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-credentials-api-openapi.yml
- filename: sifflet-dbt-integration-api-openapi.yml
  format: yaml
  label: Sifflet dbt integration API
  slug: sifflet-dbt-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-dbt-integration-api-openapi.yml
- filename: sifflet-declarative-assets-and-lineage-api-openapi.yml
  format: yaml
  label: Sifflet Declarative Assets and Lineage API
  slug: sifflet-declarative-assets-and-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-declarative-assets-and-lineage-api-openapi.yml
- filename: sifflet-domains-api-openapi.yml
  format: yaml
  label: Sifflet Domains API
  slug: sifflet-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-domains-api-openapi.yml
- filename: sifflet-external-catalog-api-openapi.yml
  format: yaml
  label: Sifflet External Catalog API
  slug: sifflet-external-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-external-catalog-api-openapi.yml
- filename: sifflet-notification-rules-api-openapi.yml
  format: yaml
  label: Sifflet Notification Rules API
  slug: sifflet-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-notification-rules-api-openapi.yml
- filename: sifflet-rule-api-openapi.yml
  format: yaml
  label: Sifflet Rule API
  slug: sifflet-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-rule-api-openapi.yml
- filename: sifflet-rule-run-api-openapi.yml
  format: yaml
  label: Sifflet Rule Run API
  slug: sifflet-rule-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-rule-run-api-openapi.yml
- filename: sifflet-sources-deprecated-api-openapi.yml
  format: yaml
  label: Sifflet Sources (deprecated) API
  slug: sifflet-sources-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-sources-deprecated-api-openapi.yml
- filename: sifflet-sources-v2-api-openapi.yml
  format: yaml
  label: Sifflet Sources (v2) API
  slug: sifflet-sources-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-sources-v2-api-openapi.yml
- filename: sifflet-teams-api-openapi.yml
  format: yaml
  label: Sifflet Teams API
  slug: sifflet-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-teams-api-openapi.yml
- filename: sifflet-users-api-openapi.yml
  format: yaml
  label: Sifflet Users API
  slug: sifflet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-users-api-openapi.yml
- filename: sifflet-workspace-api-openapi.yml
  format: yaml
  label: Sifflet Workspace API
  slug: sifflet-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: siffletdata.com
  spf: true
hosts:
- cert_expires: Oct 16 07:11:02 2026 GMT
  host: www.siffletdata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sifflet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sifflet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sifflet
provider_slug: sifflet
slug: sifflet-domain-security
source_filename: sifflet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siffletdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 07:11:02 2026 GMT\n  hsts: false\ndomains:\n- domain: siffletdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/security/sifflet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Analytics
- Data Observability
- Data Quality
- Data Catalog
- Data Lineage
- Data Governance
- Monitoring
- Metadata
- AI Agents
---
