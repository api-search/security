---
api_specs:
- filename: gotowebinar-attendees-api-openapi.yml
  format: yaml
  label: GoToWebinar Attendees API
  slug: gotowebinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-attendees-api-openapi.yml
- filename: gotowebinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoToWebinar Co-Organizers API
  slug: gotowebinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-co-organizers-api-openapi.yml
- filename: gotowebinar-panelists-api-openapi.yml
  format: yaml
  label: GoToWebinar Panelists API
  slug: gotowebinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-panelists-api-openapi.yml
- filename: gotowebinar-polls-api-openapi.yml
  format: yaml
  label: GoToWebinar Polls API
  slug: gotowebinar-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-polls-api-openapi.yml
- filename: gotowebinar-questions-api-openapi.yml
  format: yaml
  label: GoToWebinar Questions API
  slug: gotowebinar-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-questions-api-openapi.yml
- filename: gotowebinar-recordings-api-openapi.yml
  format: yaml
  label: GoToWebinar Recordings API
  slug: gotowebinar-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-recordings-api-openapi.yml
- filename: gotowebinar-registrants-api-openapi.yml
  format: yaml
  label: GoToWebinar Registrants API
  slug: gotowebinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-registrants-api-openapi.yml
- filename: gotowebinar-sessions-api-openapi.yml
  format: yaml
  label: GoToWebinar Sessions API
  slug: gotowebinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-sessions-api-openapi.yml
- filename: gotowebinar-surveys-api-openapi.yml
  format: yaml
  label: GoToWebinar Surveys API
  slug: gotowebinar-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-surveys-api-openapi.yml
- filename: gotowebinar-user-subscriptions-api-openapi.yml
  format: yaml
  label: GoToWebinar User Subscriptions API
  slug: gotowebinar-user-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-user-subscriptions-api-openapi.yml
- filename: gotowebinar-webhooks-api-openapi.yml
  format: yaml
  label: GoToWebinar Webhooks API
  slug: gotowebinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webhooks-api-openapi.yml
- filename: gotowebinar-webinars-api-openapi.yml
  format: yaml
  label: GoToWebinar Webinars API
  slug: gotowebinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webinars-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getgo.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developer.goto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: api.getgo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gotowebinar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoToWebinar, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoToWebinar
provider_slug: gotowebinar
slug: gotowebinar-domain-security
source_filename: gotowebinar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.goto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getgo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getgo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/security/gotowebinar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Attendees
- Collaboration
- Communications
- Events
- Meetings
- Registrants
- Sessions
- Surveys
- Video Conferencing
- Virtual Events
- Webhooks
- Webinars
---
