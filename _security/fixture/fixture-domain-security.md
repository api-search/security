---
api_specs:
- filename: fixture-accounts-api-openapi.yml
  format: yaml
  label: Fixture Accounts API
  slug: fixture-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-accounts-api-openapi.yml
- filename: fixture-activities-api-openapi.yml
  format: yaml
  label: Fixture Activities API
  slug: fixture-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-activities-api-openapi.yml
- filename: fixture-contacts-api-openapi.yml
  format: yaml
  label: Fixture Contacts API
  slug: fixture-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-contacts-api-openapi.yml
- filename: fixture-deals-api-openapi.yml
  format: yaml
  label: Fixture Deals API
  slug: fixture-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-deals-api-openapi.yml
- filename: fixture-fixture-api-api-openapi.yml
  format: yaml
  label: Fixture Fixture API API
  slug: fixture-fixture-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-fixture-api-api-openapi.yml
- filename: fixture-leads-api-openapi.yml
  format: yaml
  label: Fixture Leads API
  slug: fixture-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-leads-api-openapi.yml
- filename: fixture-notes-api-openapi.yml
  format: yaml
  label: Fixture Notes API
  slug: fixture-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-notes-api-openapi.yml
- filename: fixture-pipelines-api-openapi.yml
  format: yaml
  label: Fixture Pipelines API
  slug: fixture-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-pipelines-api-openapi.yml
- filename: fixture-task-statuses-api-openapi.yml
  format: yaml
  label: Fixture Task Statuses API
  slug: fixture-task-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-task-statuses-api-openapi.yml
- filename: fixture-tasks-api-openapi.yml
  format: yaml
  label: Fixture Tasks API
  slug: fixture-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-tasks-api-openapi.yml
- filename: fixture-users-api-openapi.yml
  format: yaml
  label: Fixture Users API
  slug: fixture-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fixture.app
  spf: true
hosts:
- cert_expires: Aug 23 12:56:41 2026 GMT
  host: fixture.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 10:14:41 2026 GMT
  host: beta-api.fixture.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fixture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixture, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fixture
provider_slug: fixture
slug: fixture-domain-security
source_filename: fixture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixture.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:56:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: beta-api.fixture.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:14:41 2026 GMT\n  hsts: null\ndomains:\n- domain: fixture.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/security/fixture-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- CRM
- Sales
- B2B
- Artificial Intelligence
- Agents
- MCP
- Customer Relationship Management
---
