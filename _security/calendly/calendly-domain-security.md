---
api_specs:
- filename: calendly-webhook-api-asyncapi.yml
  format: yaml
  label: Calendly Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/calendly/asyncapi/calendly-webhook-api-asyncapi.yml
- filename: calendly-availability-api-openapi.yml
  format: yaml
  label: Calendly Availability API
  slug: calendly-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-availability-api-openapi.yml
- filename: calendly-groups-api-openapi.yml
  format: yaml
  label: Calendly Groups API
  slug: calendly-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-groups-api-openapi.yml
- filename: calendly-organizations-api-openapi.yml
  format: yaml
  label: Calendly Organizations API
  slug: calendly-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-organizations-api-openapi.yml
- filename: calendly-shares-api-openapi.yml
  format: yaml
  label: Calendly Shares API
  slug: calendly-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-shares-api-openapi.yml
- filename: calendly-users-api-openapi.yml
  format: yaml
  label: Calendly Users API
  slug: calendly-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-users-api-openapi.yml
- filename: calendly-activitylog-api-openapi.yml
  format: yaml
  label: Calendly Activity Log API
  slug: calendly-activitylog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-activitylog-api-openapi.yml
- filename: calendly-contacts-api-openapi.yml
  format: yaml
  label: Calendly Contacts API
  slug: calendly-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-contacts-api-openapi.yml
- filename: calendly-datacompliance-api-openapi.yml
  format: yaml
  label: Calendly Data Compliance API
  slug: calendly-datacompliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-datacompliance-api-openapi.yml
- filename: calendly-eventtypes-api-openapi.yml
  format: yaml
  label: Calendly Event Types API
  slug: calendly-eventtypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-eventtypes-api-openapi.yml
- filename: calendly-locations-api-openapi.yml
  format: yaml
  label: Calendly Locations API
  slug: calendly-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-locations-api-openapi.yml
- filename: calendly-notetaker-api-openapi.yml
  format: yaml
  label: Calendly Notetaker API
  slug: calendly-notetaker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-notetaker-api-openapi.yml
- filename: calendly-outgoingcommunications-api-openapi.yml
  format: yaml
  label: Calendly Outgoing Communications API
  slug: calendly-outgoingcommunications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-outgoingcommunications-api-openapi.yml
- filename: calendly-routingforms-api-openapi.yml
  format: yaml
  label: Calendly Routing Forms API
  slug: calendly-routingforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-routingforms-api-openapi.yml
- filename: calendly-scheduledevents-api-openapi.yml
  format: yaml
  label: Calendly Scheduled Events API
  slug: calendly-scheduledevents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-scheduledevents-api-openapi.yml
- filename: calendly-webhooks-api-openapi.yml
  format: yaml
  label: Calendly Webhooks API
  slug: calendly-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-webhooks-api-openapi.yml
- filename: calendly-scheduling-links-api-openapi.yml
  format: yaml
  label: Calendly Scheduling Links API
  slug: calendly-scheduling-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-scheduling-links-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:platform@calendly.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: calendly.com
  spf: true
hosts:
- cert_expires: Oct  5 14:35:08 2026 GMT
  host: developer.calendly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:35:08 2026 GMT
  host: calendly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:35:08 2026 GMT
  host: api.calendly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Calendly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calendly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Calendly
provider_slug: calendly
slug: calendly-domain-security
source_filename: calendly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.calendly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: calendly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.calendly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:35:08 2026 GMT\n  hsts: null\ndomains:\n- domain: calendly.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:platform@calendly.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/calendly/security/calendly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Appointments
- Automation
- Booking
- Calendar
- Meetings
- Scheduling
---
