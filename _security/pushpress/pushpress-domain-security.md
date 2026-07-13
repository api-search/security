---
api_specs:
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Customers API
  slug: pushpress-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Check-Ins API
  slug: pushpress-checkins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Appointments API
  slug: pushpress-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Classes API
  slug: pushpress-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Events API
  slug: pushpress-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Enrollments and Plans API
  slug: pushpress-enrollments-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Company API
  slug: pushpress-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Invitations API
  slug: pushpress-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Messaging API
  slug: pushpress-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Webhooks API
  slug: pushpress-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress API Keys API
  slug: pushpress-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pushpress.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:spf.mandrillapp.com include:sendgrid.net include:1711513.spf10.hubspotemail.net ~all
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.pushpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: awselb/2.0
  tls_version: TLSv1.3
- cert_expires: Sep  6 00:27:39 2026 GMT
  host: api.pushpress.com
  hsts: false
  https: true
  note: Root path returns 404; API is served under /v3 with API-KEY and company-id headers.
  server: nginx/1.25.5
  tls_version: TLSv1.3
- cert_expires: Sep  6 00:27:39 2026 GMT
  host: developer.pushpress.com
  hsts: false
  https: true
  note: Redirects to /dashboard/login (developer portal).
  server: nginx/1.25.5
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pushpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PushPress, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PushPress
provider_slug: pushpress
slug: pushpress-domain-security
source_filename: pushpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API + docs hosts\nhosts:\n- host: www.pushpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: awselb/2.0\n- host: api.pushpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:27:39 2026 GMT\n  hsts: false\n  server: nginx/1.25.5\n  note: Root path returns 404; API is served under /v3 with API-KEY and company-id headers.\n- host: developer.pushpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:27:39 2026 GMT\n  hsts: false\n  server: nginx/1.25.5\n  note: Redirects to /dashboard/login (developer portal).\ndomains:\n- domain: pushpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:amazonses.com include:spf.mandrillapp.com include:sendgrid.net include:1711513.spf10.hubspotemail.net ~all'\n  dmarc: true\n\
  \  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/security/pushpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Gym Management
- Membership Management
- Fitness Software
- Class Scheduling
- Billing
- CRM
- Wellness
- SaaS
- Webhooks
---
