---
api_specs:
- filename: agorapulse-calendar-notes-api-openapi.yml
  format: yaml
  label: Agorapulse Calendar Notes API
  slug: agorapulse-calendar-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-calendar-notes-api-openapi.yml
- filename: agorapulse-inbox-conversations-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox conversations API
  slug: agorapulse-inbox-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-conversations-api-openapi.yml
- filename: agorapulse-inbox-items-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox items API
  slug: agorapulse-inbox-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-items-api-openapi.yml
- filename: agorapulse-inbox-reply-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox reply API
  slug: agorapulse-inbox-reply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-reply-api-openapi.yml
- filename: agorapulse-openapi-api-openapi.yml
  format: yaml
  label: Agorapulse OpenAPI API
  slug: agorapulse-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-openapi-api-openapi.yml
- filename: agorapulse-organization-api-openapi.yml
  format: yaml
  label: Agorapulse Organization API
  slug: agorapulse-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-organization-api-openapi.yml
- filename: agorapulse-profile-api-openapi.yml
  format: yaml
  label: Agorapulse Profile API
  slug: agorapulse-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-profile-api-openapi.yml
- filename: agorapulse-report-api-openapi.yml
  format: yaml
  label: Agorapulse Report API
  slug: agorapulse-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-report-api-openapi.yml
- filename: agorapulse-simple-drafts-api-openapi.yml
  format: yaml
  label: Agorapulse Simple Drafts API
  slug: agorapulse-simple-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-simple-drafts-api-openapi.yml
- filename: agorapulse-simple-scheduling-api-openapi.yml
  format: yaml
  label: Agorapulse Simple Scheduling API
  slug: agorapulse-simple-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-simple-scheduling-api-openapi.yml
- filename: agorapulse-studio-media-api-openapi.yml
  format: yaml
  label: Agorapulse Studio Media API
  slug: agorapulse-studio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-studio-media-api-openapi.yml
- filename: agorapulse-workspace-api-openapi.yml
  format: yaml
  label: Agorapulse Workspace API
  slug: agorapulse-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-workspace-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: agorapulse.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.agorapulse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: support.agorapulse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.agorapulse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agorapulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agorapulse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agorapulse
provider_slug: agorapulse
slug: agorapulse-domain-security
source_filename: agorapulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agorapulse.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/security/agorapulse-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
