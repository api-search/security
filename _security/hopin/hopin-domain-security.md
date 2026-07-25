---
api_specs:
- filename: hopin-bank-questions-api-openapi.yml
  format: yaml
  label: RingCentral Events Bank Questions API
  slug: hopin-bank-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-bank-questions-api-openapi.yml
- filename: hopin-booths-api-openapi.yml
  format: yaml
  label: RingCentral Events Booths API
  slug: hopin-booths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-booths-api-openapi.yml
- filename: hopin-data-subscriptions-api-openapi.yml
  format: yaml
  label: RingCentral Events Data Subscriptions API
  slug: hopin-data-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-data-subscriptions-api-openapi.yml
- filename: hopin-events-api-openapi.yml
  format: yaml
  label: RingCentral Events Events API
  slug: hopin-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-events-api-openapi.yml
- filename: hopin-health-api-openapi.yml
  format: yaml
  label: RingCentral Events Health API
  slug: hopin-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-health-api-openapi.yml
- filename: hopin-magic-links-api-openapi.yml
  format: yaml
  label: RingCentral Events Magic Links API
  slug: hopin-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-magic-links-api-openapi.yml
- filename: hopin-organizations-api-openapi.yml
  format: yaml
  label: RingCentral Events Organizations API
  slug: hopin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-organizations-api-openapi.yml
- filename: hopin-registrations-api-openapi.yml
  format: yaml
  label: RingCentral Events Registrations API
  slug: hopin-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-registrations-api-openapi.yml
- filename: hopin-reports-api-openapi.yml
  format: yaml
  label: RingCentral Events Reports API
  slug: hopin-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-reports-api-openapi.yml
- filename: hopin-schedule-items-api-openapi.yml
  format: yaml
  label: RingCentral Events Schedule Items API
  slug: hopin-schedule-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-schedule-items-api-openapi.yml
- filename: hopin-sessions-api-openapi.yml
  format: yaml
  label: RingCentral Events Sessions API
  slug: hopin-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-sessions-api-openapi.yml
- filename: hopin-stages-api-openapi.yml
  format: yaml
  label: RingCentral Events Stages API
  slug: hopin-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-stages-api-openapi.yml
- filename: hopin-templates-api-openapi.yml
  format: yaml
  label: RingCentral Events Templates API
  slug: hopin-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-templates-api-openapi.yml
- filename: hopin-tickets-api-openapi.yml
  format: yaml
  label: RingCentral Events Tickets API
  slug: hopin-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-tickets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ringcentral.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: developer.events.ringcentral.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 07:48:19 2026 GMT
  host: api.events.ringcentral.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hopin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RingCentral Events, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RingCentral Events
provider_slug: hopin
slug: hopin-domain-security
source_filename: hopin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.events.ringcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.events.ringcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ringcentral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/security/hopin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
---
