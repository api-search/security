---
api_specs:
- filename: chili-piper-availability-api-openapi.yml
  format: yaml
  label: Chili Piper Availability API
  slug: chili-piper-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-availability-api-openapi.yml
- filename: chili-piper-chat-api-openapi.yml
  format: yaml
  label: Chili Piper Chat API
  slug: chili-piper-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-chat-api-openapi.yml
- filename: chili-piper-concierge-api-openapi.yml
  format: yaml
  label: Chili Piper Concierge API
  slug: chili-piper-concierge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-concierge-api-openapi.yml
- filename: chili-piper-distribution-api-openapi.yml
  format: yaml
  label: Chili Piper Distribution API
  slug: chili-piper-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distribution-api-openapi.yml
- filename: chili-piper-distro-api-openapi.yml
  format: yaml
  label: Chili Piper Distro API
  slug: chili-piper-distro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distro-api-openapi.yml
- filename: chili-piper-handoff-api-openapi.yml
  format: yaml
  label: Chili Piper Handoff API
  slug: chili-piper-handoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-handoff-api-openapi.yml
- filename: chili-piper-meeting-type-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type API
  slug: chili-piper-meeting-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-api-openapi.yml
- filename: chili-piper-meeting-type-reminder-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type Reminder API
  slug: chili-piper-meeting-type-reminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-reminder-api-openapi.yml
- filename: chili-piper-meetings-api-openapi.yml
  format: yaml
  label: Chili Piper Meetings API
  slug: chili-piper-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meetings-api-openapi.yml
- filename: chili-piper-rule-api-openapi.yml
  format: yaml
  label: Chili Piper Rule API
  slug: chili-piper-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-rule-api-openapi.yml
- filename: chili-piper-schedulinglinks-api-openapi.yml
  format: yaml
  label: Chili Piper Scheduling Links API
  slug: chili-piper-schedulinglinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-schedulinglinks-api-openapi.yml
- filename: chili-piper-team-api-openapi.yml
  format: yaml
  label: Chili Piper Team API
  slug: chili-piper-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-team-api-openapi.yml
- filename: chili-piper-tenant-api-openapi.yml
  format: yaml
  label: Chili Piper Tenant API
  slug: chili-piper-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-tenant-api-openapi.yml
- filename: chili-piper-user-api-openapi.yml
  format: yaml
  label: Chili Piper User API
  slug: chili-piper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-user-api-openapi.yml
- filename: chili-piper-workspace-api-openapi.yml
  format: yaml
  label: Chili Piper Workspace API
  slug: chili-piper-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-workspace-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "gogetssl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chilipiper.com
  spf: true
hosts:
- cert_expires: Sep 27 05:09:40 2026 GMT
  host: www.chilipiper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:42:25 2026 GMT
  host: help.chilipiper.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 05:09:40 2026 GMT
  host: fire.chilipiper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chili Piper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chili Piper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chili Piper
provider_slug: chili-piper
slug: chili-piper-domain-security
source_filename: chili-piper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chilipiper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.chilipiper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:42:25 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: fire.chilipiper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:09:40 2026 GMT\n  hsts: null\ndomains:\n- domain: chilipiper.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"gogetssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/security/chili-piper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Lead Routing
- Meetings
- Sales
- Marketing
- CRM
- Demand Conversion
- Appointment Booking
- Revenue Operations
- Calendar
- Agents
- MCP
---
