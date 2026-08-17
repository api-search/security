---
api_specs:
- filename: agorapulse-calendar-notes-api-openapi.yml
  format: yaml
  label: Agorapulse Calendar Notes API
  slug: agorapulse-calendar-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-calendar-notes-api-openapi.yml
- filename: agorapulse-agorapulse-api-api-openapi.yml
  format: yaml
  label: Agorapulse Webhooks API
  slug: agorapulse-agorapulse-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-agorapulse-api-api-openapi.yml
- filename: agorapulse-competitor-api-openapi.yml
  format: yaml
  label: Agorapulse Competitor API
  slug: agorapulse-competitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-competitor-api-openapi.yml
- filename: agorapulse-conversations-api-openapi.yml
  format: yaml
  label: Agorapulse Conversations API
  slug: agorapulse-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-conversations-api-openapi.yml
- filename: agorapulse-drafts-api-openapi.yml
  format: yaml
  label: Agorapulse Drafts API
  slug: agorapulse-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-drafts-api-openapi.yml
- filename: agorapulse-groups-api-openapi.yml
  format: yaml
  label: Agorapulse Groups API
  slug: agorapulse-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-groups-api-openapi.yml
- filename: agorapulse-health-api-openapi.yml
  format: yaml
  label: Agorapulse Health API
  slug: agorapulse-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-health-api-openapi.yml
- filename: agorapulse-items-api-openapi.yml
  format: yaml
  label: Agorapulse Items API
  slug: agorapulse-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-items-api-openapi.yml
- filename: agorapulse-media-api-openapi.yml
  format: yaml
  label: Agorapulse Media API
  slug: agorapulse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-media-api-openapi.yml
- filename: agorapulse-organizations-api-openapi.yml
  format: yaml
  label: Agorapulse Organizations API
  slug: agorapulse-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-organizations-api-openapi.yml
- filename: agorapulse-pinterest-boards-api-openapi.yml
  format: yaml
  label: Agorapulse Pinterest boards API
  slug: agorapulse-pinterest-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-pinterest-boards-api-openapi.yml
- filename: agorapulse-profiles-api-openapi.yml
  format: yaml
  label: Agorapulse Profiles API
  slug: agorapulse-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-profiles-api-openapi.yml
- filename: agorapulse-replies-api-openapi.yml
  format: yaml
  label: Agorapulse Replies API
  slug: agorapulse-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-replies-api-openapi.yml
- filename: agorapulse-reports-api-openapi.yml
  format: yaml
  label: Agorapulse Reports API
  slug: agorapulse-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-reports-api-openapi.yml
- filename: agorapulse-workspaces-api-openapi.yml
  format: yaml
  label: Agorapulse Workspaces API
  slug: agorapulse-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
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
overview: 'Domain security posture for Agorapulse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agorapulse
provider_slug: agorapulse
slug: agorapulse-domain-security
source_filename: agorapulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agorapulse.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/security/agorapulse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
