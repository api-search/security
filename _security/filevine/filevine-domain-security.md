---
api_specs:
- filename: filevine-identity-api-openapi.yml
  format: yaml
  label: Filevine Identity API
  slug: filevine-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-identity-api-openapi.yml
- filename: filevine-projects-api-openapi.yml
  format: yaml
  label: Filevine Projects API
  slug: filevine-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-projects-api-openapi.yml
- filename: filevine-contacts-api-openapi.yml
  format: yaml
  label: Filevine Contacts API
  slug: filevine-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-contacts-api-openapi.yml
- filename: filevine-documents-api-openapi.yml
  format: yaml
  label: Filevine Documents API
  slug: filevine-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-documents-api-openapi.yml
- filename: filevine-notes-api-openapi.yml
  format: yaml
  label: Filevine Notes API
  slug: filevine-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-notes-api-openapi.yml
- filename: filevine-deadlines-api-openapi.yml
  format: yaml
  label: Filevine Deadlines API
  slug: filevine-deadlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-deadlines-api-openapi.yml
- filename: filevine-tasks-api-openapi.yml
  format: yaml
  label: Filevine Tasks API
  slug: filevine-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-tasks-api-openapi.yml
- filename: filevine-time-entries-api-openapi.yml
  format: yaml
  label: Filevine Time Entries API
  slug: filevine-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-time-entries-api-openapi.yml
- filename: filevine-webhooks-api-openapi.yml
  format: yaml
  label: Filevine Webhooks API
  slug: filevine-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: filevine.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: filevine.io
  spf: false
hosts:
- cert_expires: Oct  4 21:45:30 2026 GMT
  host: www.filevine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:40:57 2026 GMT
  host: support.filevine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:34:43 2026 GMT
  host: developer.filevine.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Filevine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filevine, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Filevine
provider_slug: filevine
slug: filevine-domain-security
source_filename: filevine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.filevine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:45:30 2026 GMT\n  hsts: false\n- host: support.filevine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.filevine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:34:43 2026 GMT\n  hsts: null\ndomains:\n- domain: filevine.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: filevine.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/security/filevine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal
- Case Management
- Matters
- Intake
- Documents
- LOIS
- Webhooks
- Legal AI
- Personal Injury
- Mass Torts
---
