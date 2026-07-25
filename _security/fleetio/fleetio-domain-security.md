---
api_specs:
- filename: fleetio-contacts-api-openapi.yml
  format: yaml
  label: Fleetio Contacts API
  slug: fleetio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-contacts-api-openapi.yml
- filename: fleetio-fuel-entries-api-openapi.yml
  format: yaml
  label: Fleetio Fuel Entries API
  slug: fleetio-fuel-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-fuel-entries-api-openapi.yml
- filename: fleetio-inspections-api-openapi.yml
  format: yaml
  label: Fleetio Inspections API
  slug: fleetio-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-inspections-api-openapi.yml
- filename: fleetio-inventory-journal-entries-api-openapi.yml
  format: yaml
  label: Fleetio Inventory Journal Entries API
  slug: fleetio-inventory-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-inventory-journal-entries-api-openapi.yml
- filename: fleetio-issues-api-openapi.yml
  format: yaml
  label: Fleetio Issues API
  slug: fleetio-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-issues-api-openapi.yml
- filename: fleetio-parts-api-openapi.yml
  format: yaml
  label: Fleetio Parts API
  slug: fleetio-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-parts-api-openapi.yml
- filename: fleetio-service-entries-api-openapi.yml
  format: yaml
  label: Fleetio Service Entries API
  slug: fleetio-service-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-service-entries-api-openapi.yml
- filename: fleetio-service-reminders-api-openapi.yml
  format: yaml
  label: Fleetio Service Reminders API
  slug: fleetio-service-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-service-reminders-api-openapi.yml
- filename: fleetio-vehicles-api-openapi.yml
  format: yaml
  label: Fleetio Vehicles API
  slug: fleetio-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-vehicles-api-openapi.yml
- filename: fleetio-webhooks-api-openapi.yml
  format: yaml
  label: Fleetio Webhooks API
  slug: fleetio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-webhooks-api-openapi.yml
- filename: fleetio-work-orders-api-openapi.yml
  format: yaml
  label: Fleetio Work Orders API
  slug: fleetio-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-work-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fleetio.com
  spf: true
hosts:
- cert_expires: Aug  8 22:52:46 2026 GMT
  host: www.fleetio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 17:53:49 2026 GMT
  host: developer.fleetio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 20:49:29 2026 GMT
  host: secure.fleetio.com
  hsts: true
  hsts_max_age: 2629746
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fleetio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fleetio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fleetio
provider_slug: fleetio
slug: fleetio-domain-security
source_filename: fleetio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fleetio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 22:52:46 2026 GMT\n  hsts: null\n- host: developer.fleetio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:53:49 2026 GMT\n  hsts: false\n- host: secure.fleetio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:49:29 2026 GMT\n  hsts: true\n  hsts_max_age: 2629746\ndomains:\n- domain: fleetio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/security/fleetio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Vehicles
- Maintenance
- Telematics
- SaaS
---
