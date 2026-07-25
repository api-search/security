---
api_specs:
- filename: race-entry-event-api-openapi.yml
  format: yaml
  label: Race Entry Event API
  slug: race-entry-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-event-api-openapi.yml
- filename: race-entry-get-category-teams-api-openapi.yml
  format: yaml
  label: Race Entry Get Category Teams API
  slug: race-entry-get-category-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-category-teams-api-openapi.yml
- filename: race-entry-get-event-categories-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Categories API
  slug: race-entry-get-event-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-categories-api-openapi.yml
- filename: race-entry-get-event-participants-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Participants API
  slug: race-entry-get-event-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-participants-api-openapi.yml
- filename: race-entry-get-event-pin-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Pin API
  slug: race-entry-get-event-pin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-pin-api-openapi.yml
- filename: race-entry-get-event-questions-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Questions API
  slug: race-entry-get-event-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-questions-api-openapi.yml
- filename: race-entry-get-event-teams-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Teams API
  slug: race-entry-get-event-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-teams-api-openapi.yml
- filename: race-entry-get-events-api-openapi.yml
  format: yaml
  label: Race Entry Get Events API
  slug: race-entry-get-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-events-api-openapi.yml
- filename: race-entry-login-api-openapi.yml
  format: yaml
  label: Race Entry Login API
  slug: race-entry-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-login-api-openapi.yml
- filename: race-entry-memberships-api-openapi.yml
  format: yaml
  label: Race Entry Memberships API
  slug: race-entry-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-memberships-api-openapi.yml
- filename: race-entry-result-api-openapi.yml
  format: yaml
  label: Race Entry Result API
  slug: race-entry-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-result-api-openapi.yml
- filename: race-entry-set-event-app-access-api-openapi.yml
  format: yaml
  label: Race Entry Set Event App Access API
  slug: race-entry-set-event-app-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-set-event-app-access-api-openapi.yml
- filename: race-entry-set-event-pin-api-openapi.yml
  format: yaml
  label: Race Entry Set Event Pin API
  slug: race-entry-set-event-pin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-set-event-pin-api-openapi.yml
- filename: race-entry-update-event-participant-api-openapi.yml
  format: yaml
  label: Race Entry Update Event Participant API
  slug: race-entry-update-event-participant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-update-event-participant-api-openapi.yml
- filename: race-entry-upload-api-openapi.yml
  format: yaml
  label: Race Entry Upload API
  slug: race-entry-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-upload-api-openapi.yml
- filename: race-entry-user-api-openapi.yml
  format: yaml
  label: Race Entry User API
  slug: race-entry-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: raceentry.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: www.raceentry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 14:24:00 2026 GMT
  host: demo.raceentry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Race Entry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Race Entry, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Race Entry
provider_slug: race-entry
slug: race-entry-domain-security
source_filename: race-entry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raceentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.raceentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:24:00 2026 GMT\n  hsts: false\ndomains:\n- domain: raceentry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/security/race-entry-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Race Timing
- Race Registration
- Event Management
- Race Results
- Sports
---
