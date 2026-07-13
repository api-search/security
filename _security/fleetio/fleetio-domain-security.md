---
api_specs:
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Vehicles API
  slug: vehicles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Fuel Entries API
  slug: fuel-entries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Service & Work Orders API
  slug: service-work-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Parts & Inventory API
  slug: parts-inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Inspections API
  slug: inspections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
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
