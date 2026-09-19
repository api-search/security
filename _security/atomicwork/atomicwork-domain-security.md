---
api_specs:
- filename: atomicwork-assets-api-openapi.yml
  format: yaml
  label: Atomicwork assets API
  slug: atomicwork-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-assets-api-openapi.yml
- filename: atomicwork-businesshourconfig-api-openapi.yml
  format: yaml
  label: Atomicwork businessHourConfig API
  slug: atomicwork-businesshourconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-businesshourconfig-api-openapi.yml
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
- filename: atomicwork-access-management-api-openapi.yml
  format: yaml
  label: Atomicwork Access Management API
  slug: atomicwork-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-access-management-api-openapi.yml
- filename: atomicwork-agent-groups-api-openapi.yml
  format: yaml
  label: Atomicwork Agent Groups API
  slug: atomicwork-agent-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-agent-groups-api-openapi.yml
- filename: atomicwork-audit-logs-api-openapi.yml
  format: yaml
  label: Atomicwork Audit Logs API
  slug: atomicwork-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-audit-logs-api-openapi.yml
- filename: atomicwork-change-management-api-openapi.yml
  format: yaml
  label: Atomicwork Change Management API
  slug: atomicwork-change-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-change-management-api-openapi.yml
- filename: atomicwork-custom-objects-api-openapi.yml
  format: yaml
  label: Atomicwork Custom Objects API
  slug: atomicwork-custom-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-custom-objects-api-openapi.yml
- filename: atomicwork-service-catalog-api-openapi.yml
  format: yaml
  label: Atomicwork Service Catalog API
  slug: atomicwork-service-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-service-catalog-api-openapi.yml
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
hosts_probed: 2
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
