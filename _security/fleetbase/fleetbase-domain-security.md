---
api_specs:
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Places API
  slug: places
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Drivers & Vehicles API
  slug: drivers-vehicles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Fleets & Zones API
  slug: fleets-zones
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Service Rates API
  slug: service-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Tracking API
  slug: tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fleetbase.io
  spf: false
hosts:
- cert_expires: Oct  8 01:09:33 2026 GMT
  host: www.fleetbase.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 00:19:49 2026 GMT
  host: docs.fleetbase.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.fleetbase.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fleetbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fleetbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Fleetbase
provider_slug: fleetbase
slug: fleetbase-domain-security
source_filename: fleetbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fleetbase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:09:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fleetbase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:19:49 2026 GMT\n  hsts: false\n- host: api.fleetbase.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fleetbase.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/security/fleetbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Fleet Management
- Supply Chain
- Last Mile Delivery
- Open Source
---
