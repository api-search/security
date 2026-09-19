---
api_specs:
- filename: flightfinder-aircraft-api-openapi.yml
  format: yaml
  label: FlightFinder Aircraft API
  slug: flightfinder-aircraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-aircraft-api-openapi.yml
- filename: flightfinder-airports-api-openapi.yml
  format: yaml
  label: FlightFinder Airports API
  slug: flightfinder-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-airports-api-openapi.yml
- filename: flightfinder-drone-sightings-api-openapi.yml
  format: yaml
  label: FlightFinder Drone Sightings API
  slug: flightfinder-drone-sightings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-drone-sightings-api-openapi.yml
- filename: flightfinder-events-api-openapi.yml
  format: yaml
  label: FlightFinder Events API
  slug: flightfinder-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-events-api-openapi.yml
- filename: flightfinder-keys-api-openapi.yml
  format: yaml
  label: FlightFinder Keys API
  slug: flightfinder-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-keys-api-openapi.yml
- filename: flightfinder-laser-strikes-api-openapi.yml
  format: yaml
  label: FlightFinder Laser Strikes API
  slug: flightfinder-laser-strikes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-laser-strikes-api-openapi.yml
- filename: flightfinder-narratives-api-openapi.yml
  format: yaml
  label: FlightFinder Narratives API
  slug: flightfinder-narratives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-narratives-api-openapi.yml
- filename: flightfinder-ping-api-openapi.yml
  format: yaml
  label: FlightFinder Ping API
  slug: flightfinder-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-ping-api-openapi.yml
- filename: flightfinder-sources-api-openapi.yml
  format: yaml
  label: FlightFinder Sources API
  slug: flightfinder-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-sources-api-openapi.yml
- filename: flightfinder-wildlife-strikes-api-openapi.yml
  format: yaml
  label: FlightFinder Wildlife Strikes API
  slug: flightfinder-wildlife-strikes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/openapi/flightfinder-wildlife-strikes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: himaxym.com
  spf: true
hosts:
- cert_expires: Nov 16 07:43:07 2026 GMT
  host: himaxym.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flightfinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlightFinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FlightFinder
provider_slug: flightfinder
slug: flightfinder-domain-security
source_filename: flightfinder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: himaxym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 07:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: himaxym.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/security/flightfinder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Aviation Safety
- Accident Data
- Open Data
- Public Domain
- Transportation
- Government Data
- Research
- Reference Data
- Agent Ready
---
