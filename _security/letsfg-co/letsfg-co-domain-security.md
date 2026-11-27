---
api_specs:
- filename: letsfg-co-agents-api-openapi.yml
  format: yaml
  label: LetsFG Agents API
  slug: letsfg-co-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-agents-api-openapi.yml
- filename: letsfg-co-flights-api-openapi.yml
  format: yaml
  label: LetsFG Flights API
  slug: letsfg-co-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-flights-api-openapi.yml
- filename: letsfg-co-hotels-api-openapi.yml
  format: yaml
  label: LetsFG Hotels API
  slug: letsfg-co-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-hotels-api-openapi.yml
- filename: letsfg-co-sandbox-api-openapi.yml
  format: yaml
  label: LetsFG Sandbox API
  slug: letsfg-co-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-sandbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: letsfg.co
  spf: true
hosts:
- cert_expires: Dec 19 19:38:33 2026 GMT
  host: letsfg.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LetsFG Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LetsFG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LetsFG
provider_slug: letsfg-co
slug: letsfg-co-domain-security
source_filename: letsfg-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letsfg.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 19:38:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: letsfg.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/letsfg-co/security/letsfg-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Artificial Intelligence
- Booking
- Flights
- Hotels
---
