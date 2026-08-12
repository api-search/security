---
api_specs:
- filename: zoom-meeting--openapi-original.yml
  format: yaml
  label: Zoom Meeting API
  slug: zoom-meeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/_original/zoom-meeting--openapi-original.yml
- filename: zoom-account-api-openapi.yml
  format: yaml
  label: Zoom Account API
  slug: zoom-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-account-api-openapi.yml
- filename: zoom-chat-api-openapi.yml
  format: yaml
  label: Zoom Chat API
  slug: zoom-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-chat-api-openapi.yml
- filename: zoom-cloud-recording-api-openapi.yml
  format: yaml
  label: Zoom Cloud Recording API
  slug: zoom-cloud-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-cloud-recording-api-openapi.yml
- filename: zoom-dashboard-api-openapi.yml
  format: yaml
  label: Zoom Dashboard API
  slug: zoom-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-dashboard-api-openapi.yml
- filename: zoom-device-api-openapi.yml
  format: yaml
  label: Zoom Device API
  slug: zoom-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-device-api-openapi.yml
- filename: zoom-group-api-openapi.yml
  format: yaml
  label: Zoom Group API
  slug: zoom-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-group-api-openapi.yml
- filename: zoom-im-group-api-openapi.yml
  format: yaml
  label: Zoom IM Group API
  slug: zoom-im-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-im-group-api-openapi.yml
- filename: zoom-meeting-live-stream-api-openapi.yml
  format: yaml
  label: Zoom Meeting Live Stream API
  slug: zoom-meeting-live-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting-live-stream-api-openapi.yml
- filename: zoom-meeting-participants-api-openapi.yml
  format: yaml
  label: Zoom Meeting Participants API
  slug: zoom-meeting-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting-participants-api-openapi.yml
- filename: zoom-meeting-polls-api-openapi.yml
  format: yaml
  label: Zoom Meeting Polls API
  slug: zoom-meeting-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting-polls-api-openapi.yml
- filename: zoom-meeting-recordings-api-openapi.yml
  format: yaml
  label: Zoom Meeting Recordings API
  slug: zoom-meeting-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting-recordings-api-openapi.yml
- filename: zoom-meeting-registrants-api-openapi.yml
  format: yaml
  label: Zoom Meeting Registrants API
  slug: zoom-meeting-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting-registrants-api-openapi.yml
- filename: zoom-meetings-api-openapi.yml
  format: yaml
  label: Zoom Meetings API
  slug: zoom-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meetings-api-openapi.yml
- filename: zoom-report-api-openapi.yml
  format: yaml
  label: Zoom Report API
  slug: zoom-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-report-api-openapi.yml
- filename: zoom-user-api-openapi.yml
  format: yaml
  label: Zoom User API
  slug: zoom-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-user-api-openapi.yml
- filename: zoom-webinar-api-openapi.yml
  format: yaml
  label: Zoom Webinar API
  slug: zoom-webinar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-webinar-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@zoom.us"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoom.us
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: developers.zoom.us
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.zoom.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoom, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoom
provider_slug: zoom
slug: zoom-domain-security
source_filename: zoom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.zoom.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n- host: api.zoom.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zoom.us\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@zoom.us\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/security/zoom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
---
