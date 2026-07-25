---
api_specs:
- filename: spot-analytics-api-openapi.yml
  format: yaml
  label: Spot Analytics API
  slug: spot-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-analytics-api-openapi.yml
- filename: spot-appliances-api-openapi.yml
  format: yaml
  label: Spot Appliances API
  slug: spot-appliances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-appliances-api-openapi.yml
- filename: spot-audio-api-openapi.yml
  format: yaml
  label: Spot Audio API
  slug: spot-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-audio-api-openapi.yml
- filename: spot-cameras-api-openapi.yml
  format: yaml
  label: Spot Cameras API
  slug: spot-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-cameras-api-openapi.yml
- filename: spot-embeds-api-openapi.yml
  format: yaml
  label: Spot Embeds API
  slug: spot-embeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-embeds-api-openapi.yml
- filename: spot-historical-footage-api-openapi.yml
  format: yaml
  label: Spot Historical Footage API
  slug: spot-historical-footage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-historical-footage-api-openapi.yml
- filename: spot-integration-devices-api-openapi.yml
  format: yaml
  label: Spot Integration Devices API
  slug: spot-integration-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integration-devices-api-openapi.yml
- filename: spot-integration-event-types-api-openapi.yml
  format: yaml
  label: Spot Integration Event Types API
  slug: spot-integration-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integration-event-types-api-openapi.yml
- filename: spot-integration-events-api-openapi.yml
  format: yaml
  label: Spot Integration Events API
  slug: spot-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integration-events-api-openapi.yml
- filename: spot-integrations-api-openapi.yml
  format: yaml
  label: Spot Integrations API
  slug: spot-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integrations-api-openapi.yml
- filename: spot-locations-api-openapi.yml
  format: yaml
  label: Spot Locations API
  slug: spot-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-locations-api-openapi.yml
- filename: spot-lpi-api-openapi.yml
  format: yaml
  label: Spot LPI API
  slug: spot-lpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-lpi-api-openapi.yml
- filename: spot-lpr-api-openapi.yml
  format: yaml
  label: Spot LPR API
  slug: spot-lpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-lpr-api-openapi.yml
- filename: spot-shared-search-api-openapi.yml
  format: yaml
  label: Spot Shared Search API
  slug: spot-shared-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-shared-search-api-openapi.yml
- filename: spot-zones-api-openapi.yml
  format: yaml
  label: Spot Zones API
  slug: spot-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spot.ai
  spf: true
hosts:
- cert_expires: Sep 28 18:10:06 2026 GMT
  host: www.spot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 22:31:40 2026 GMT
  host: developers.spot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:44:12 2026 GMT
  host: dev-api.spot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spot
provider_slug: spot
slug: spot-domain-security
source_filename: spot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-api.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:44:12 2026 GMT\n  hsts: null\ndomains:\n- domain: spot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/security/spot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Physical Security
- Surveillance
- Computer Vision
- Artificial Intelligence
- Cameras
- Analytics
- License Plate Recognition
- Webhooks
- Integrations
---
