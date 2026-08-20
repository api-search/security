---
api_specs:
- filename: goto-webinar-openapi.yml
  format: yaml
  label: GoTo Webinar REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/_original/goto-webinar-openapi.yml
- filename: goto-webinar-attendees-api-openapi.yml
  format: yaml
  label: GoTo Webinar Attendees API
  slug: goto-webinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-attendees-api-openapi.yml
- filename: goto-webinar-panelists-api-openapi.yml
  format: yaml
  label: GoTo Webinar Panelists API
  slug: goto-webinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-panelists-api-openapi.yml
- filename: goto-webinar-registrants-api-openapi.yml
  format: yaml
  label: GoTo Webinar Registrants API
  slug: goto-webinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-registrants-api-openapi.yml
- filename: goto-webinar-sessions-api-openapi.yml
  format: yaml
  label: GoTo Webinar Sessions API
  slug: goto-webinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-sessions-api-openapi.yml
- filename: goto-webinar-webinars-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webinars API
  slug: goto-webinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webinars-api-openapi.yml
- filename: goto-webinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoTo Webinar Co Organizers API
  slug: goto-webinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-co-organizers-api-openapi.yml
- filename: goto-webinar-recordingassets-api-openapi.yml
  format: yaml
  label: GoTo Webinar Recording Assets API
  slug: goto-webinar-recordingassets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-recordingassets-api-openapi.yml
- filename: goto-webinar-webhooks-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webhooks API
  slug: goto-webinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webhooks-api-openapi.yml
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
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.goto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
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
name: Goto Webinar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoTo Webinar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoTo Webinar
provider_slug: goto-webinar
slug: goto-webinar-domain-security
source_filename: goto-webinar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: developer.goto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getgo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getgo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/security/goto-webinar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
- Webhook
- Event Management
- Collaboration
- Analytics
---
