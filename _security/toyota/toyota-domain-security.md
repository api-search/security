---
api_specs:
- filename: toyota-climate-api-openapi.yml
  format: yaml
  label: Toyota Climate API
  slug: toyota-climate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-climate-api-openapi.yml
- filename: toyota-electric-api-openapi.yml
  format: yaml
  label: Toyota Electric API
  slug: toyota-electric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-electric-api-openapi.yml
- filename: toyota-fleet-api-openapi.yml
  format: yaml
  label: Toyota Fleet API
  slug: toyota-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-fleet-api-openapi.yml
- filename: toyota-health-api-openapi.yml
  format: yaml
  label: Toyota Health API
  slug: toyota-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-health-api-openapi.yml
- filename: toyota-history-api-openapi.yml
  format: yaml
  label: Toyota History API
  slug: toyota-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-history-api-openapi.yml
- filename: toyota-location-api-openapi.yml
  format: yaml
  label: Toyota Location API
  slug: toyota-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-location-api-openapi.yml
- filename: toyota-notifications-api-openapi.yml
  format: yaml
  label: Toyota Notifications API
  slug: toyota-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-notifications-api-openapi.yml
- filename: toyota-remote-api-openapi.yml
  format: yaml
  label: Toyota Remote API
  slug: toyota-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-remote-api-openapi.yml
- filename: toyota-status-api-openapi.yml
  format: yaml
  label: Toyota Status API
  slug: toyota-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-status-api-openapi.yml
- filename: toyota-subscriptions-api-openapi.yml
  format: yaml
  label: Toyota Subscriptions API
  slug: toyota-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-subscriptions-api-openapi.yml
- filename: toyota-telemetry-api-openapi.yml
  format: yaml
  label: Toyota Telemetry API
  slug: toyota-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-telemetry-api-openapi.yml
- filename: toyota-trips-api-openapi.yml
  format: yaml
  label: Toyota Trips API
  slug: toyota-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-trips-api-openapi.yml
- filename: toyota-vehicles-api-openapi.yml
  format: yaml
  label: Toyota Vehicles API
  slug: toyota-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-vehicles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toyota.com
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: developer.eig.toyota.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: developer-sb.eig.toyota.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.toyota.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toyota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toyota, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toyota
provider_slug: toyota
slug: toyota-domain-security
source_filename: toyota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.eig.toyota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\n- host: developer-sb.eig.toyota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.toyota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: toyota.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/security/toyota-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automobiles
- Cars
- Vehicles
- Connected Car
- Telematics
- Fleet Management
- Electric Vehicles
---
