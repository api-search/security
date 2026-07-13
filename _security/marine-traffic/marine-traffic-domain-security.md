---
api_specs:
- filename: marine-traffic-vessel-positions-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Positions API
  slug: marine-traffic-vessel-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-positions-openapi.yml
- filename: marine-traffic-events-openapi.yml
  format: yaml
  label: MarineTraffic Events API
  slug: marine-traffic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-events-openapi.yml
- filename: marine-traffic-vessels-data-openapi.yml
  format: yaml
  label: MarineTraffic Vessels Data API
  slug: marine-traffic-vessels-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessels-data-openapi.yml
- filename: marine-traffic-voyage-info-openapi.yml
  format: yaml
  label: MarineTraffic Voyage Information API
  slug: marine-traffic-voyage-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-voyage-info-openapi.yml
- filename: marine-traffic-ports-info-openapi.yml
  format: yaml
  label: MarineTraffic Ports Information API
  slug: marine-traffic-ports-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-ports-info-openapi.yml
- filename: marine-traffic-routing-openapi.yml
  format: yaml
  label: MarineTraffic Routing Information API
  slug: marine-traffic-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-routing-openapi.yml
- filename: marine-traffic-reverse-geocoding-openapi.yml
  format: yaml
  label: MarineTraffic Reverse Geocoding API
  slug: marine-traffic-reverse-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-reverse-geocoding-openapi.yml
- filename: marine-traffic-power-user-openapi.yml
  format: yaml
  label: MarineTraffic Power User API
  slug: marine-traffic-power-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-power-user-openapi.yml
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
