---
api_specs:
- filename: velaris-activity-api-openapi.yml
  format: yaml
  label: Velaris Activity API
  slug: velaris-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-activity-api-openapi.yml
- filename: velaris-attribute-change-log-api-openapi.yml
  format: yaml
  label: Velaris Attribute Change Log API
  slug: velaris-attribute-change-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-attribute-change-log-api-openapi.yml
- filename: velaris-currencies-api-openapi.yml
  format: yaml
  label: Velaris Currencies API
  slug: velaris-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-currencies-api-openapi.yml
- filename: velaris-custom-objects-api-openapi.yml
  format: yaml
  label: Velaris Custom Objects API
  slug: velaris-custom-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-custom-objects-api-openapi.yml
- filename: velaris-entity-management-v1-api-openapi.yml
  format: yaml
  label: Velaris Entity Management V1 API
  slug: velaris-entity-management-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-entity-management-v1-api-openapi.yml
- filename: velaris-entity-management-v2-api-openapi.yml
  format: yaml
  label: Velaris Entity Management V2 API
  slug: velaris-entity-management-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-entity-management-v2-api-openapi.yml
- filename: velaris-field-definitions-api-openapi.yml
  format: yaml
  label: Velaris Field Definitions API
  slug: velaris-field-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-field-definitions-api-openapi.yml
- filename: velaris-integrations-api-openapi.yml
  format: yaml
  label: Velaris Integrations API
  slug: velaris-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-integrations-api-openapi.yml
- filename: velaris-lifecycles-api-openapi.yml
  format: yaml
  label: Velaris Lifecycles API
  slug: velaris-lifecycles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-lifecycles-api-openapi.yml
- filename: velaris-notes-api-openapi.yml
  format: yaml
  label: Velaris Notes API
  slug: velaris-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-notes-api-openapi.yml
- filename: velaris-surveys-api-openapi.yml
  format: yaml
  label: Velaris Surveys API
  slug: velaris-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-surveys-api-openapi.yml
- filename: velaris-tasks-api-openapi.yml
  format: yaml
  label: Velaris Tasks API
  slug: velaris-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-tasks-api-openapi.yml
- filename: velaris-ticketing-api-openapi.yml
  format: yaml
  label: Velaris Ticketing API
  slug: velaris-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-ticketing-api-openapi.yml
- filename: velaris-users-api-openapi.yml
  format: yaml
  label: Velaris Users API
  slug: velaris-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: velaris.io
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.euw1.velaris.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velaris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velaris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Velaris
provider_slug: velaris
slug: velaris-domain-security
source_filename: velaris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.euw1.velaris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: velaris.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/security/velaris-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Success
- AI
- SaaS
- Customer Data
- CRM
- Analytics
- Automation
- Company
---
