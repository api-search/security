---
api_specs:
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Calendars API
  slug: calendars
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Events API
  slug: events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Smart Invites API
  slug: smart-invites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Scheduling Links API
  slug: scheduling-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Push Notifications API
  slug: push-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:ops@cronofy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cronofy.com
  spf: true
hosts:
- cert_expires: Sep 15 05:45:57 2026 GMT
  host: www.cronofy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: docs.cronofy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.cronofy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cronofy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cronofy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cronofy
provider_slug: cronofy
slug: cronofy-domain-security
source_filename: cronofy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cronofy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cronofy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cronofy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cronofy.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:ops@cronofy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/security/cronofy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Calendar
- Availability
- Booking
- Productivity
---
