---
api_specs:
- filename: hubilo-event-api-openapi.yml
  format: yaml
  label: hubilo Event API
  slug: hubilo-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-event-api-openapi.yml
- filename: hubilo-exhibitor-api-openapi.yml
  format: yaml
  label: hubilo Exhibitor API
  slug: hubilo-exhibitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-exhibitor-api-openapi.yml
- filename: hubilo-organiser-api-openapi.yml
  format: yaml
  label: hubilo Organiser API
  slug: hubilo-organiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-organiser-api-openapi.yml
- filename: hubilo-session-api-openapi.yml
  format: yaml
  label: hubilo Session API
  slug: hubilo-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-session-api-openapi.yml
- filename: hubilo-speaker-api-openapi.yml
  format: yaml
  label: hubilo Speaker API
  slug: hubilo-speaker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-speaker-api-openapi.yml
- filename: hubilo-upload-media-api-openapi.yml
  format: yaml
  label: hubilo Upload Media API
  slug: hubilo-upload-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-upload-media-api-openapi.yml
- filename: hubilo-user-api-openapi.yml
  format: yaml
  label: hubilo User API
  slug: hubilo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hubilo.com
  spf: true
hosts:
- cert_expires: Sep 26 01:13:27 2026 GMT
  host: hubilo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.hubilo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hubilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hubilo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: hubilo
provider_slug: hubilo
slug: hubilo-domain-security
source_filename: hubilo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hubilo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:13:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hubilo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hubilo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/security/hubilo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Event
- Virtual Events
- Webinars
- Event Management
- Hybrid Events
- Attendee Engagement
---
