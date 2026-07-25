---
api_specs:
- filename: lunar-energy-devices-api-openapi.yml
  format: yaml
  label: Lunar Energy Devices API
  slug: lunar-energy-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-devices-api-openapi.yml
- filename: lunar-energy-diff-requests-api-openapi.yml
  format: yaml
  label: Lunar Energy Diff Requests API
  slug: lunar-energy-diff-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-diff-requests-api-openapi.yml
- filename: lunar-energy-dynamic-tariffs-api-openapi.yml
  format: yaml
  label: Lunar Energy Dynamic Tariffs API
  slug: lunar-energy-dynamic-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-dynamic-tariffs-api-openapi.yml
- filename: lunar-energy-flex-dispatches-api-openapi.yml
  format: yaml
  label: Lunar Energy Flex Dispatches API
  slug: lunar-energy-flex-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-flex-dispatches-api-openapi.yml
- filename: lunar-energy-flex-events-api-openapi.yml
  format: yaml
  label: Lunar Energy Flex Events API
  slug: lunar-energy-flex-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-flex-events-api-openapi.yml
- filename: lunar-energy-flex-groups-api-openapi.yml
  format: yaml
  label: Lunar Energy Flex Groups API
  slug: lunar-energy-flex-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-flex-groups-api-openapi.yml
- filename: lunar-energy-operation-mode-api-openapi.yml
  format: yaml
  label: Lunar Energy Operation Mode API
  slug: lunar-energy-operation-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-operation-mode-api-openapi.yml
- filename: lunar-energy-periodical-tariffs-api-openapi.yml
  format: yaml
  label: Lunar Energy Periodical Tariffs API
  slug: lunar-energy-periodical-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-periodical-tariffs-api-openapi.yml
- filename: lunar-energy-plans-api-openapi.yml
  format: yaml
  label: Lunar Energy Plans API
  slug: lunar-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-plans-api-openapi.yml
- filename: lunar-energy-prognoses-api-openapi.yml
  format: yaml
  label: Lunar Energy Prognoses API
  slug: lunar-energy-prognoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-prognoses-api-openapi.yml
- filename: lunar-energy-sites-api-openapi.yml
  format: yaml
  label: Lunar Energy Sites API
  slug: lunar-energy-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-sites-api-openapi.yml
- filename: lunar-energy-telemetry-api-openapi.yml
  format: yaml
  label: Lunar Energy Telemetry API
  slug: lunar-energy-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-telemetry-api-openapi.yml
- filename: lunar-energy-visits-api-openapi.yml
  format: yaml
  label: Lunar Energy Visits API
  slug: lunar-energy-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/lunar-energy-visits-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lunarenergy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gridshare.com
  spf: true
hosts:
- cert_expires: Oct  4 05:50:21 2026 GMT
  host: www.lunarenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:47:11 2026 GMT
  host: www.gridshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:18:19 2026 GMT
  host: developers.gridshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunar Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunar Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lunar Energy
provider_slug: lunar-energy
slug: lunar-energy-domain-security
source_filename: lunar-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lunarenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:50:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.gridshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:47:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.gridshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:18:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lunarenergy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gridshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/security/lunar-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Home Battery
- Solar
- Virtual Power Plant
- DERMS
- Distributed Energy Resources
- Grid Services
- Demand Response
- Storage
- Inverter
- Smart Home
- Energy Management
- Tariffs
- Telemetry
- VPP
- Flex Events
---
