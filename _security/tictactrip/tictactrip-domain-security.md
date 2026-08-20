---
api_specs:
- filename: tictactrip-autocomplete-api-openapi.yml
  format: yaml
  label: TicTacTrip Autocomplete API
  slug: tictactrip-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-autocomplete-api-openapi.yml
- filename: tictactrip-booking-api-openapi.yml
  format: yaml
  label: TicTacTrip Booking API
  slug: tictactrip-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-booking-api-openapi.yml
- filename: tictactrip-cities-api-openapi.yml
  format: yaml
  label: TicTacTrip Cities API
  slug: tictactrip-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-cities-api-openapi.yml
- filename: tictactrip-results-api-openapi.yml
  format: yaml
  label: TicTacTrip Results API
  slug: tictactrip-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-results-api-openapi.yml
- filename: tictactrip-segmentproviders-api-openapi.yml
  format: yaml
  label: TicTacTrip SegmentProviders API
  slug: tictactrip-segmentproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-segmentproviders-api-openapi.yml
- filename: tictactrip-stopclusters-api-openapi.yml
  format: yaml
  label: TicTacTrip StopClusters API
  slug: tictactrip-stopclusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-stopclusters-api-openapi.yml
- filename: tictactrip-stopgroups-api-openapi.yml
  format: yaml
  label: TicTacTrip StopGroups API
  slug: tictactrip-stopgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-stopgroups-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tictactrip.eu
  spf: true
hosts:
- cert_expires: Sep 24 18:22:29 2026 GMT
  host: tictactrip.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tictactrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TicTacTrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TicTacTrip
provider_slug: tictactrip
slug: tictactrip-domain-security
source_filename: tictactrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tictactrip.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:22:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tictactrip.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/security/tictactrip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Transportation
- Trains
- Bus
- Booking
- Mobility
- Multi-Modal
- Ticketing
---
