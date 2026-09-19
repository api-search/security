---
api_specs:
- filename: configure8-catalog-entities-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entities API
  slug: configure8-catalog-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entities-api-openapi.yml
- filename: configure8-catalog-relations-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relations API
  slug: configure8-catalog-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relations-api-openapi.yml
- filename: configure8-deployments-api-openapi.yml
  format: yaml
  label: Configure8 Deployments API
  slug: configure8-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployments-api-openapi.yml
- filename: configure8-scorecards-api-openapi.yml
  format: yaml
  label: Configure8 Scorecards API
  slug: configure8-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecards-api-openapi.yml
- filename: configure8-users-api-openapi.yml
  format: yaml
  label: Configure8 Users API
  slug: configure8-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-users-api-openapi.yml
- filename: configure8-catalog-entity-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entity API
  slug: configure8-catalog-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entity-api-openapi.yml
- filename: configure8-catalog-entity-batch-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entity Batch API
  slug: configure8-catalog-entity-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entity-batch-api-openapi.yml
- filename: configure8-catalog-entity-metadata-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entity Metadata API
  slug: configure8-catalog-entity-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entity-metadata-api-openapi.yml
- filename: configure8-catalog-relation-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relation API
  slug: configure8-catalog-relation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relation-api-openapi.yml
- filename: configure8-credential-api-openapi.yml
  format: yaml
  label: Configure8 Credential API
  slug: configure8-credential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-credential-api-openapi.yml
- filename: configure8-deployment-api-openapi.yml
  format: yaml
  label: Configure8 Deployment API
  slug: configure8-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployment-api-openapi.yml
- filename: configure8-module-settings-api-openapi.yml
  format: yaml
  label: Configure8 Module Settings API
  slug: configure8-module-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-module-settings-api-openapi.yml
- filename: configure8-private-scim-api-openapi.yml
  format: yaml
  label: Configure8 Private SCIM API
  slug: configure8-private-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-private-scim-api-openapi.yml
- filename: configure8-scim-api-openapi.yml
  format: yaml
  label: Configure8 SCIM API
  slug: configure8-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scim-api-openapi.yml
- filename: configure8-scorecard-api-openapi.yml
  format: yaml
  label: Configure8 Scorecard API
  slug: configure8-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecard-api-openapi.yml
- filename: configure8-sync-api-openapi.yml
  format: yaml
  label: Configure8 Sync API
  slug: configure8-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-sync-api-openapi.yml
- filename: configure8-templates-api-openapi.yml
  format: yaml
  label: Configure8 Templates API
  slug: configure8-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: configure8.io
  spf: false
hosts:
- cert_expires: Nov  6 11:36:04 2026 GMT
  host: www.configure8.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: app.configure8.io
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Configure8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Configure8, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Configure8
provider_slug: configure8
slug: configure8-domain-security
source_filename: configure8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.configure8.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 11:36:04 2026 GMT\n  hsts: false\n- host: app.configure8.io\n  https: false\ndomains:\n- domain: configure8.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/security/configure8-domain-security.yml
summary_line: TLSv1.3
tags:
- Catalog
- Cloud Cost
- Developer Experience
- DevOps
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Service Catalog
- SRE
---
