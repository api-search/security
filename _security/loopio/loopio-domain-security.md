---
api_specs:
- filename: loopio-asynchronous-api-openapi.yml
  format: yaml
  label: Loopio Asynchronous API
  slug: loopio-asynchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-asynchronous-api-openapi.yml
- filename: loopio-crm-api-openapi.yml
  format: yaml
  label: Loopio CRM API
  slug: loopio-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-crm-api-openapi.yml
- filename: loopio-custom-project-fields-api-openapi.yml
  format: yaml
  label: Loopio Custom Project Fields API
  slug: loopio-custom-project-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-custom-project-fields-api-openapi.yml
- filename: loopio-customers-api-openapi.yml
  format: yaml
  label: Loopio Customers API
  slug: loopio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-customers-api-openapi.yml
- filename: loopio-files-api-openapi.yml
  format: yaml
  label: Loopio Files API
  slug: loopio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-files-api-openapi.yml
- filename: loopio-library-entries-api-openapi.yml
  format: yaml
  label: Loopio Library Entries API
  slug: loopio-library-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-library-entries-api-openapi.yml
- filename: loopio-merge-variables-api-openapi.yml
  format: yaml
  label: Loopio Merge Variables API
  slug: loopio-merge-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-merge-variables-api-openapi.yml
- filename: loopio-project-templates-api-openapi.yml
  format: yaml
  label: Loopio Project Templates API
  slug: loopio-project-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-project-templates-api-openapi.yml
- filename: loopio-projects-api-openapi.yml
  format: yaml
  label: Loopio Projects API
  slug: loopio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-projects-api-openapi.yml
- filename: loopio-roles-api-openapi.yml
  format: yaml
  label: Loopio Roles API
  slug: loopio-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-roles-api-openapi.yml
- filename: loopio-stacks-api-openapi.yml
  format: yaml
  label: Loopio Stacks API
  slug: loopio-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-stacks-api-openapi.yml
- filename: loopio-tags-api-openapi.yml
  format: yaml
  label: Loopio Tags API
  slug: loopio-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-tags-api-openapi.yml
- filename: loopio-teams-api-openapi.yml
  format: yaml
  label: Loopio Teams API
  slug: loopio-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-teams-api-openapi.yml
- filename: loopio-users-api-openapi.yml
  format: yaml
  label: Loopio Users API
  slug: loopio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-users-api-openapi.yml
- filename: loopio-webhooks-api-openapi.yml
  format: yaml
  label: Loopio Webhooks API
  slug: loopio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: loopio.com
  spf: true
hosts:
- cert_expires: Oct  8 23:37:04 2026 GMT
  host: loopio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: developer.loopio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.loopio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loopio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loopio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Loopio
provider_slug: loopio
slug: loopio-domain-security
source_filename: loopio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loopio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:37:04 2026 GMT\n  hsts: false\n- host: developer.loopio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.loopio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: loopio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/security/loopio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- RFP
- Proposals
- Response Management
- Content Library
- Sales Enablement
- Questionnaires
- Compliance
- Collaboration
- Documents
- Webhook
- Software-as-a-Service
---
