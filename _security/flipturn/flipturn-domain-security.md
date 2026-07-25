---
api_specs:
- filename: flipturn-access-ids-api-openapi.yml
  format: yaml
  label: Flipturn Access IDs API
  slug: flipturn-access-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-access-ids-api-openapi.yml
- filename: flipturn-alerts-api-openapi.yml
  format: yaml
  label: Flipturn Alerts API
  slug: flipturn-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-alerts-api-openapi.yml
- filename: flipturn-charger-health-api-openapi.yml
  format: yaml
  label: Flipturn Charger Health API
  slug: flipturn-charger-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-charger-health-api-openapi.yml
- filename: flipturn-chargers-api-openapi.yml
  format: yaml
  label: Flipturn Chargers API
  slug: flipturn-chargers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-chargers-api-openapi.yml
- filename: flipturn-charging-sessions-api-openapi.yml
  format: yaml
  label: Flipturn Charging Sessions API
  slug: flipturn-charging-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-charging-sessions-api-openapi.yml
- filename: flipturn-departure-times-api-openapi.yml
  format: yaml
  label: Flipturn Departure Times API
  slug: flipturn-departure-times-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-departure-times-api-openapi.yml
- filename: flipturn-errors-api-openapi.yml
  format: yaml
  label: Flipturn Errors API
  slug: flipturn-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-errors-api-openapi.yml
- filename: flipturn-maintenance-windows-api-openapi.yml
  format: yaml
  label: Flipturn Maintenance Windows API
  slug: flipturn-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-maintenance-windows-api-openapi.yml
- filename: flipturn-ocpp-messages-api-openapi.yml
  format: yaml
  label: Flipturn OCPP Messages API
  slug: flipturn-ocpp-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-ocpp-messages-api-openapi.yml
- filename: flipturn-reservations-api-openapi.yml
  format: yaml
  label: Flipturn Reservations API
  slug: flipturn-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-reservations-api-openapi.yml
- filename: flipturn-site-power-limits-api-openapi.yml
  format: yaml
  label: Flipturn Site Power Limits API
  slug: flipturn-site-power-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-site-power-limits-api-openapi.yml
- filename: flipturn-sites-api-openapi.yml
  format: yaml
  label: Flipturn Sites API
  slug: flipturn-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-sites-api-openapi.yml
- filename: flipturn-vehicles-api-openapi.yml
  format: yaml
  label: Flipturn Vehicles API
  slug: flipturn-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-vehicles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getflipturn.com
  spf: true
hosts:
- cert_expires: Sep 12 11:57:08 2026 GMT
  host: www.getflipturn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 00:49:43 2026 GMT
  host: api.getflipturn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flipturn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipturn, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Flipturn
provider_slug: flipturn
slug: flipturn-domain-security
source_filename: flipturn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getflipturn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:57:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getflipturn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:49:43 2026 GMT\n  hsts: null\ndomains:\n- domain: getflipturn.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/security/flipturn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EV Charging
- Electric Vehicles
- Fleet Management
- Energy
- Charging Infrastructure
- OCPP
- OCPI
- Mobility
- REST API
---
