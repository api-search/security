---
api_specs:
- filename: marine-traffic-ais-api-api-openapi.yml
  format: yaml
  label: MarineTraffic AIS API API
  slug: marine-traffic-ais-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-ais-api-api-openapi.yml
- filename: marine-traffic-balances-api-openapi.yml
  format: yaml
  label: MarineTraffic Balances API
  slug: marine-traffic-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-balances-api-openapi.yml
- filename: marine-traffic-fleets-api-openapi.yml
  format: yaml
  label: MarineTraffic Fleets API
  slug: marine-traffic-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-fleets-api-openapi.yml
- filename: marine-traffic-passage-plans-api-openapi.yml
  format: yaml
  label: MarineTraffic Passage Plans API
  slug: marine-traffic-passage-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-passage-plans-api-openapi.yml
- filename: marine-traffic-port-events-api-openapi.yml
  format: yaml
  label: MarineTraffic Port Events API
  slug: marine-traffic-port-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-port-events-api-openapi.yml
- filename: marine-traffic-ports-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Ports Information API
  slug: marine-traffic-ports-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-ports-information-api-openapi.yml
- filename: marine-traffic-reverse-geocoding-api-openapi.yml
  format: yaml
  label: MarineTraffic Reverse Geocoding API
  slug: marine-traffic-reverse-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-reverse-geocoding-api-openapi.yml
- filename: marine-traffic-routing-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Routing Information API
  slug: marine-traffic-routing-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-routing-information-api-openapi.yml
- filename: marine-traffic-search-vessel-api-openapi.yml
  format: yaml
  label: MarineTraffic Search Vessel API
  slug: marine-traffic-search-vessel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-search-vessel-api-openapi.yml
- filename: marine-traffic-single-vessel-events-api-openapi.yml
  format: yaml
  label: MarineTraffic Single Vessel Events API
  slug: marine-traffic-single-vessel-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-single-vessel-events-api-openapi.yml
- filename: marine-traffic-vessel-historical-track-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Historical Track API
  slug: marine-traffic-vessel-historical-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-historical-track-api-openapi.yml
- filename: marine-traffic-vessel-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Information API
  slug: marine-traffic-vessel-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-information-api-openapi.yml
- filename: marine-traffic-vessel-positions-legacy-api-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Positions (Legacy API) API
  slug: marine-traffic-vessel-positions-legacy-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-positions-legacy-api-api-openapi.yml
- filename: marine-traffic-voyage-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Voyage Information API
  slug: marine-traffic-voyage-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-voyage-information-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marinetraffic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kpler.com
  spf: true
hosts:
- cert_expires: Oct  8 18:34:35 2026 GMT
  host: www.marinetraffic.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 02:44:31 2026 GMT
  host: www.kpler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 17:54:15 2026 GMT
  host: servicedocs.marinetraffic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marine Traffic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarineTraffic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MarineTraffic
provider_slug: marine-traffic
slug: marine-traffic-domain-security
source_filename: marine-traffic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marinetraffic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.kpler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: servicedocs.marinetraffic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:54:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marinetraffic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kpler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/security/marine-traffic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIS
- Maritime
- Vessel Tracking
- Shipping
- Ports
- Voyage Forecasting
- Geospatial
- Kpler
---
