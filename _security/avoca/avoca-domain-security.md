---
api_specs:
- filename: avoca-analytics-v1-api-openapi.yml
  format: yaml
  label: Avoca Analytics (v1) API
  slug: avoca-analytics-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-analytics-v1-api-openapi.yml
- filename: avoca-calls-api-openapi.yml
  format: yaml
  label: Avoca Calls API
  slug: avoca-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-calls-api-openapi.yml
- filename: avoca-coach-api-openapi.yml
  format: yaml
  label: Avoca Coach API
  slug: avoca-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-coach-api-openapi.yml
- filename: avoca-leads-api-openapi.yml
  format: yaml
  label: Avoca Leads API
  slug: avoca-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-leads-api-openapi.yml
- filename: avoca-outbound-texting-api-openapi.yml
  format: yaml
  label: Avoca Outbound Texting API
  slug: avoca-outbound-texting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-outbound-texting-api-openapi.yml
- filename: avoca-scheduler-analytics-v0-api-openapi.yml
  format: yaml
  label: Avoca Scheduler Analytics (v0) API
  slug: avoca-scheduler-analytics-v0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-scheduler-analytics-v0-api-openapi.yml
- filename: avoca-sessions-bookings-api-openapi.yml
  format: yaml
  label: Avoca Sessions & Bookings API
  slug: avoca-sessions-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-sessions-bookings-api-openapi.yml
- filename: avoca-teams-api-openapi.yml
  format: yaml
  label: Avoca Teams API
  slug: avoca-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avoca.ai
  spf: true
hosts:
- cert_expires: Oct 15 22:14:12 2026 GMT
  host: docs.avoca.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 11:09:40 2026 GMT
  host: enterprise-api.avoca.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avoca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avoca, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avoca
provider_slug: avoca
slug: avoca-domain-security
source_filename: avoca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.avoca.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:14:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: enterprise-api.avoca.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:09:40 2026 GMT\n  hsts: null\ndomains:\n- domain: avoca.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/security/avoca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Voice AI
- Conversational AI
- Customer Service
- Contact Center
- Home Services
- Field Service
- Scheduling
- Analytics
- Webhooks
- Enterprise API
---
