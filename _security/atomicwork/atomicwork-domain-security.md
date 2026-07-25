---
api_specs:
- filename: atomicwork-accessmanagement-api-openapi.yml
  format: yaml
  label: Atomicwork accessManagement API
  slug: atomicwork-accessmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-accessmanagement-api-openapi.yml
- filename: atomicwork-agentgroups-api-openapi.yml
  format: yaml
  label: Atomicwork agentGroups API
  slug: atomicwork-agentgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-agentgroups-api-openapi.yml
- filename: atomicwork-assets-api-openapi.yml
  format: yaml
  label: Atomicwork assets API
  slug: atomicwork-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-assets-api-openapi.yml
- filename: atomicwork-auditlogs-api-openapi.yml
  format: yaml
  label: Atomicwork auditLogs API
  slug: atomicwork-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-auditlogs-api-openapi.yml
- filename: atomicwork-businesshourconfig-api-openapi.yml
  format: yaml
  label: Atomicwork businessHourConfig API
  slug: atomicwork-businesshourconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-businesshourconfig-api-openapi.yml
- filename: atomicwork-changemanagement-api-openapi.yml
  format: yaml
  label: Atomicwork changeManagement API
  slug: atomicwork-changemanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-changemanagement-api-openapi.yml
- filename: atomicwork-customobjects-api-openapi.yml
  format: yaml
  label: Atomicwork customObjects API
  slug: atomicwork-customobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-customobjects-api-openapi.yml
- filename: atomicwork-entities-api-openapi.yml
  format: yaml
  label: Atomicwork entities API
  slug: atomicwork-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-entities-api-openapi.yml
- filename: atomicwork-forms-api-openapi.yml
  format: yaml
  label: Atomicwork forms API
  slug: atomicwork-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-forms-api-openapi.yml
- filename: atomicwork-problems-api-openapi.yml
  format: yaml
  label: Atomicwork problems API
  slug: atomicwork-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-problems-api-openapi.yml
- filename: atomicwork-requests-api-openapi.yml
  format: yaml
  label: Atomicwork requests API
  slug: atomicwork-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-requests-api-openapi.yml
- filename: atomicwork-servicecatalog-api-openapi.yml
  format: yaml
  label: Atomicwork serviceCatalog API
  slug: atomicwork-servicecatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-servicecatalog-api-openapi.yml
- filename: atomicwork-tags-api-openapi.yml
  format: yaml
  label: Atomicwork tags API
  slug: atomicwork-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-tags-api-openapi.yml
- filename: atomicwork-users-api-openapi.yml
  format: yaml
  label: Atomicwork users API
  slug: atomicwork-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-users-api-openapi.yml
- filename: atomicwork-workflows-api-openapi.yml
  format: yaml
  label: Atomicwork workflows API
  slug: atomicwork-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-workflows-api-openapi.yml
- filename: atomicwork-workspaces-api-openapi.yml
  format: yaml
  label: Atomicwork workspaces API
  slug: atomicwork-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atomicwork.com
  spf: true
hosts:
- cert_expires: Aug 27 20:16:15 2026 GMT
  host: www.atomicwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 03:51:46 2026 GMT
  host: developers.atomicwork.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomicwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomicwork, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atomicwork
provider_slug: atomicwork
slug: atomicwork-domain-security
source_filename: atomicwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atomicwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.atomicwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:51:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atomicwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/security/atomicwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Service Management
- ITSM
- ESM
- IT Service Desk
- Identity Governance
- Asset Management
- AI Agents
- MCP
- Enterprise
---
