---
api_specs:
- filename: live-nation-entertainment-ticketmaster-discovery-api-openapi.yml
  format: yaml
  label: Ticketmaster Discovery API
  slug: ticketmaster-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/openapi/live-nation-entertainment-ticketmaster-discovery-api-openapi.yml
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
- cert_expires: Sep 11 19:22:12 2026 GMT
  host: app.ticketmaster.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Live Nation Entertainment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for live-nation-entertainment, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: live-nation-entertainment
provider_slug: live-nation-entertainment
slug: live-nation-entertainment-domain-security
source_filename: live-nation-entertainment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ticketmaster.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: app.ticketmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:22:12 2026 GMT\n  hsts: null\ndomains:\n- domain: ticketmaster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/security/live-nation-entertainment-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fortune 500
---
