---
api_specs:
- filename: lightfield-accounts-api-openapi.yml
  format: yaml
  label: Lightfield Accounts API
  slug: lightfield-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-accounts-api-openapi.yml
- filename: lightfield-auth-api-openapi.yml
  format: yaml
  label: Lightfield Auth API
  slug: lightfield-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-auth-api-openapi.yml
- filename: lightfield-contacts-api-openapi.yml
  format: yaml
  label: Lightfield Contacts API
  slug: lightfield-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-contacts-api-openapi.yml
- filename: lightfield-emails-api-openapi.yml
  format: yaml
  label: Lightfield Emails API
  slug: lightfield-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-emails-api-openapi.yml
- filename: lightfield-files-api-openapi.yml
  format: yaml
  label: Lightfield Files API
  slug: lightfield-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-files-api-openapi.yml
- filename: lightfield-lists-api-openapi.yml
  format: yaml
  label: Lightfield Lists API
  slug: lightfield-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-lists-api-openapi.yml
- filename: lightfield-meetings-api-openapi.yml
  format: yaml
  label: Lightfield Meetings API
  slug: lightfield-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-meetings-api-openapi.yml
- filename: lightfield-members-api-openapi.yml
  format: yaml
  label: Lightfield Members API
  slug: lightfield-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-members-api-openapi.yml
- filename: lightfield-notes-api-openapi.yml
  format: yaml
  label: Lightfield Notes API
  slug: lightfield-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-notes-api-openapi.yml
- filename: lightfield-objects-api-openapi.yml
  format: yaml
  label: Lightfield Objects API
  slug: lightfield-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-objects-api-openapi.yml
- filename: lightfield-opportunities-api-openapi.yml
  format: yaml
  label: Lightfield Opportunities API
  slug: lightfield-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-opportunities-api-openapi.yml
- filename: lightfield-tasks-api-openapi.yml
  format: yaml
  label: Lightfield Tasks API
  slug: lightfield-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-tasks-api-openapi.yml
- filename: lightfield-workflowrun-api-openapi.yml
  format: yaml
  label: Lightfield WorkflowRun API
  slug: lightfield-workflowrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-workflowrun-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightfield.app
  spf: true
hosts:
- cert_expires: Aug 23 14:10:11 2026 GMT
  host: lightfield.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:59:52 2026 GMT
  host: docs.lightfield.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.lightfield.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightfield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightfield, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lightfield
provider_slug: lightfield
slug: lightfield-domain-security
source_filename: lightfield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightfield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:10:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lightfield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:59:52 2026 GMT\n  hsts: false\n- host: api.lightfield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lightfield.app\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/security/lightfield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Application
- CRM
- Sales
- Artificial Intelligence
- Agents
- Customer Relationship Management
- Go-To-Market
- Productivity
- Software-as-a-Service
---
