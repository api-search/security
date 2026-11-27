---
api_specs:
- filename: tickets-dev-capture-api-openapi.yml
  format: yaml
  label: Tickets.dev Capture API
  slug: tickets-dev-capture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickets-dev/openapi/tickets-dev-capture-api-openapi.yml
- filename: tickets-dev-events-api-openapi.yml
  format: yaml
  label: Tickets.dev Events API
  slug: tickets-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickets-dev/openapi/tickets-dev-events-api-openapi.yml
- filename: tickets-dev-health-api-openapi.yml
  format: yaml
  label: Tickets.dev Health API
  slug: tickets-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickets-dev/openapi/tickets-dev-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tickets.dev
  spf: true
hosts:
- cert_expires: Feb  3 11:42:10 2027 GMT
  host: tickets.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tickets.dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tickets.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tickets.dev
provider_slug: tickets-dev
slug: tickets-dev-domain-security
source_filename: tickets-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tickets.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 11:42:10 2027 GMT\n  hsts: false\ndomains:\n- domain: tickets.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tickets-dev/security/tickets-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Ticketing
- Market Data
- Pricing
- Inventory
- Seat Maps
- Resale
- Event
---
