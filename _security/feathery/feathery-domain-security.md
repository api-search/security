---
api_specs:
- filename: feathery-account-api-openapi.yml
  format: yaml
  label: Feathery Account API
  slug: feathery-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-account-api-openapi.yml
- filename: feathery-data-hubs-api-openapi.yml
  format: yaml
  label: Feathery Data Hubs API
  slug: feathery-data-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-data-hubs-api-openapi.yml
- filename: feathery-document-intelligence-api-openapi.yml
  format: yaml
  label: Feathery Document Intelligence API
  slug: feathery-document-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-document-intelligence-api-openapi.yml
- filename: feathery-document-templates-api-openapi.yml
  format: yaml
  label: Feathery Document Templates API
  slug: feathery-document-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-document-templates-api-openapi.yml
- filename: feathery-end-users-api-openapi.yml
  format: yaml
  label: Feathery End Users API
  slug: feathery-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-end-users-api-openapi.yml
- filename: feathery-forms-api-openapi.yml
  format: yaml
  label: Feathery Forms API
  slug: feathery-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-forms-api-openapi.yml
- filename: feathery-hidden-fields-api-openapi.yml
  format: yaml
  label: Feathery Hidden Fields API
  slug: feathery-hidden-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-hidden-fields-api-openapi.yml
- filename: feathery-logs-api-openapi.yml
  format: yaml
  label: Feathery Logs API
  slug: feathery-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-logs-api-openapi.yml
- filename: feathery-workspaces-api-openapi.yml
  format: yaml
  label: Feathery Workspaces API
  slug: feathery-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: feathery.io
  spf: true
hosts:
- cert_expires: Oct  2 15:16:34 2026 GMT
  host: www.feathery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 23:42:41 2026 GMT
  host: api-docs.feathery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.feathery.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feathery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feathery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Feathery
provider_slug: feathery
slug: feathery-domain-security
source_filename: feathery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.feathery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:16:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.feathery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.feathery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: feathery.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/security/feathery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Form Builder
- Multi-Step Forms
- Document Intelligence
- Artificial Intelligence
- Financial-Services
- Insurance
- Wealth Management
- E-Signature
- Workflows
- Data Intake
- Submissions
- Payments
- Authentication
---
