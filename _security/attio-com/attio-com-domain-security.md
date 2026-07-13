---
api_specs:
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Objects API
  slug: attio-com-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Records API
  slug: attio-com-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Attributes API
  slug: attio-com-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Lists API
  slug: attio-com-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio List Entries API
  slug: attio-com-list-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Deals API
  slug: attio-com-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Notes API
  slug: attio-com-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Tasks API
  slug: attio-com-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Comments and Threads API
  slug: attio-com-comments-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Webhooks API
  slug: attio-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Workspace Members API
  slug: attio-com-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Meta / Self API
  slug: attio-com-meta-self-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
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
name: Attio Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Attio
provider_slug: attio-com
slug: attio-com-domain-security
source_filename: attio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 04:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:50:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 04:13:19 2026 GMT\n  hsts: null\ndomains:\n- domain: attio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/security/attio-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Customer Relationship Management
- AI
- Sales
- Data Model
- Objects and Records
---
