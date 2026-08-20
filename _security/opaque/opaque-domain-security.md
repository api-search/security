---
api_specs:
- filename: opaque-asset-configs-api-openapi.yml
  format: yaml
  label: OPAQUE Asset Configs API
  slug: opaque-asset-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-asset-configs-api-openapi.yml
- filename: opaque-auth-api-openapi.yml
  format: yaml
  label: OPAQUE Auth API
  slug: opaque-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-auth-api-openapi.yml
- filename: opaque-datasets-api-openapi.yml
  format: yaml
  label: OPAQUE Datasets API
  slug: opaque-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-datasets-api-openapi.yml
- filename: opaque-jobs-api-openapi.yml
  format: yaml
  label: OPAQUE Jobs API
  slug: opaque-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-jobs-api-openapi.yml
- filename: opaque-organizations-api-openapi.yml
  format: yaml
  label: OPAQUE Organizations API
  slug: opaque-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-organizations-api-openapi.yml
- filename: opaque-pinned-queries-api-openapi.yml
  format: yaml
  label: OPAQUE Pinned Queries API
  slug: opaque-pinned-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-pinned-queries-api-openapi.yml
- filename: opaque-predefined-query-templates-api-openapi.yml
  format: yaml
  label: OPAQUE Predefined Query Templates API
  slug: opaque-predefined-query-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-predefined-query-templates-api-openapi.yml
- filename: opaque-users-api-openapi.yml
  format: yaml
  label: OPAQUE Users API
  slug: opaque-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-users-api-openapi.yml
- filename: opaque-versioning-api-openapi.yml
  format: yaml
  label: OPAQUE Versioning API
  slug: opaque-versioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-versioning-api-openapi.yml
- filename: opaque-workflows-api-openapi.yml
  format: yaml
  label: OPAQUE Workflows API
  slug: opaque-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-workflows-api-openapi.yml
- filename: opaque-workspaces-api-openapi.yml
  format: yaml
  label: OPAQUE Workspaces API
  slug: opaque-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opaque.co
  spf: true
hosts:
- cert_expires: Oct 27 19:30:09 2026 GMT
  host: www.opaque.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 19:48:56 2026 GMT
  host: docs.opaque.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opaque Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPAQUE, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OPAQUE
provider_slug: opaque
slug: opaque-domain-security
source_filename: opaque-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnotes:\n- The apis.yml baseURL is a documented per-deployment template (https://api.{your-subdomain}/v2.5),\n  not a resolvable host, so it is excluded here. OPAQUE serves the web UI and REST API from inside\n  each customer's own environment, so only the OPAQUE-operated marketing and documentation hosts\n  are probeable from the public internet.\nhosts:\n- host: www.opaque.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 19:30:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.opaque.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:48:56 2026 GMT\n  hsts: false\ndomains:\n- domain: opaque.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/security/opaque-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Confidential Computing
- confidential-ai
- AI Governance
- Data Privacy
- Trusted Execution Environment
- Attestation
- Agentic Workflows
- Retrieval Augmented Generation
- Enterprise AI
- secure-analytics
- Data Clean Room
- MCP
---
