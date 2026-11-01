---
api_specs:
- filename: ticketsdata-openapi-generated.yml
  format: yaml
  label: TicketsData API
  slug: ticketsdata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticketsdata/openapi/_ae-authored/ticketsdata-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ticketsdata.com
  spf: true
hosts:
- cert_expires: Dec 29 17:42:52 2026 GMT
  host: ticketsdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ticketsdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TicketsData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TicketsData
provider_slug: ticketsdata
slug: ticketsdata-domain-security
source_filename: ticketsdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ticketsdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 17:42:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ticketsdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ticketsdata/security/ticketsdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ticketing
- Real-Time Data
- Market Intelligence
---
