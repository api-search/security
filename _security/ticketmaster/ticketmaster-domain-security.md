---
api_specs:
- filename: ticketmaster-discovery-openapi.yml
  format: yaml
  label: Ticketmaster Discovery API
  slug: ticketmaster-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-discovery-openapi.yml
- filename: ticketmaster-commerce-openapi.yml
  format: yaml
  label: Ticketmaster Commerce API
  slug: ticketmaster-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-commerce-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ticketmaster.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: developer.ticketmaster.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 23:25:22 2026 GMT
  host: www.ticketmaster.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 19:22:12 2026 GMT
  host: app.ticketmaster.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ticketmaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ticketmaster, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ticketmaster
provider_slug: ticketmaster
slug: ticketmaster-domain-security
source_filename: ticketmaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ticketmaster.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: www.ticketmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:25:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: app.ticketmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:22:12 2026 GMT\n  hsts: null\ndomains:\n- domain: ticketmaster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/security/ticketmaster-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Commerce
- Concerts
- Entertainment
- Events
- Sports
- Tickets
- Venues
---
