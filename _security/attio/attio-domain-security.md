---
api_specs:
- filename: attio-attributes-api-openapi.yml
  format: yaml
  label: Attio Attributes API
  slug: attio-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-attributes-api-openapi.yml
- filename: attio-call-recordings-api-openapi.yml
  format: yaml
  label: Attio Call Recordings API
  slug: attio-call-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-call-recordings-api-openapi.yml
- filename: attio-comments-api-openapi.yml
  format: yaml
  label: Attio Comments API
  slug: attio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-comments-api-openapi.yml
- filename: attio-entries-api-openapi.yml
  format: yaml
  label: Attio Entries API
  slug: attio-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-entries-api-openapi.yml
- filename: attio-files-api-openapi.yml
  format: yaml
  label: Attio Files API
  slug: attio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-files-api-openapi.yml
- filename: attio-lists-api-openapi.yml
  format: yaml
  label: Attio Lists API
  slug: attio-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-lists-api-openapi.yml
- filename: attio-meetings-api-openapi.yml
  format: yaml
  label: Attio Meetings API
  slug: attio-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-meetings-api-openapi.yml
- filename: attio-meta-api-openapi.yml
  format: yaml
  label: Attio Meta API
  slug: attio-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-meta-api-openapi.yml
- filename: attio-notes-api-openapi.yml
  format: yaml
  label: Attio Notes API
  slug: attio-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-notes-api-openapi.yml
- filename: attio-oauth-api-openapi.yml
  format: yaml
  label: Attio OAuth API
  slug: attio-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-oauth-api-openapi.yml
- filename: attio-objects-api-openapi.yml
  format: yaml
  label: Attio Objects API
  slug: attio-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-objects-api-openapi.yml
- filename: attio-records-api-openapi.yml
  format: yaml
  label: Attio Records API
  slug: attio-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-records-api-openapi.yml
- filename: attio-tasks-api-openapi.yml
  format: yaml
  label: Attio Tasks API
  slug: attio-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-tasks-api-openapi.yml
- filename: attio-threads-api-openapi.yml
  format: yaml
  label: Attio Threads API
  slug: attio-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-threads-api-openapi.yml
- filename: attio-webhooks-api-openapi.yml
  format: yaml
  label: Attio Webhooks API
  slug: attio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-webhooks-api-openapi.yml
- filename: attio-workspace-members-api-openapi.yml
  format: yaml
  label: Attio Workspace Members API
  slug: attio-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-workspace-members-api-openapi.yml
- filename: attio-list-entries-api-openapi.yml
  format: yaml
  label: Attio List Entries API
  slug: attio-list-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-list-entries-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: attio.com
  spf: true
hosts:
- cert_expires: Jul 28 04:13:19 2026 GMT
  host: attio.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:50:40 2026 GMT
  host: docs.attio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 04:13:19 2026 GMT
  host: api.attio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Attio
provider_slug: attio
slug: attio-domain-security
source_filename: attio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 04:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:50:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 04:13:19 2026 GMT\n  hsts: null\ndomains:\n- domain: attio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/security/attio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Sales
- Contacts
- Companies
- Pipeline
- Workflows
---
