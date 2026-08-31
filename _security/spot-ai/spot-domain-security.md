---
api_specs:
- filename: spot-ai-analytics-api-openapi.yml
  format: yaml
  label: Spot AI Analytics API
  slug: spot-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-analytics-api-openapi.yml
- filename: spot-ai-appliances-api-openapi.yml
  format: yaml
  label: Spot AI Appliances API
  slug: spot-ai-appliances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-appliances-api-openapi.yml
- filename: spot-ai-audio-api-openapi.yml
  format: yaml
  label: Spot AI Audio API
  slug: spot-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-audio-api-openapi.yml
- filename: spot-ai-cameras-api-openapi.yml
  format: yaml
  label: Spot AI Cameras API
  slug: spot-ai-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-cameras-api-openapi.yml
- filename: spot-ai-embeds-api-openapi.yml
  format: yaml
  label: Spot AI Embeds API
  slug: spot-ai-embeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-embeds-api-openapi.yml
- filename: spot-ai-historical-footage-api-openapi.yml
  format: yaml
  label: Spot AI Historical Footage API
  slug: spot-ai-historical-footage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-historical-footage-api-openapi.yml
- filename: spot-ai-integration-devices-api-openapi.yml
  format: yaml
  label: Spot AI Integration Devices API
  slug: spot-ai-integration-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integration-devices-api-openapi.yml
- filename: spot-ai-integration-event-types-api-openapi.yml
  format: yaml
  label: Spot AI Integration Event Types API
  slug: spot-ai-integration-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integration-event-types-api-openapi.yml
- filename: spot-ai-integration-events-api-openapi.yml
  format: yaml
  label: Spot AI Integration Events API
  slug: spot-ai-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integration-events-api-openapi.yml
- filename: spot-ai-integrations-api-openapi.yml
  format: yaml
  label: Spot AI Integrations API
  slug: spot-ai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integrations-api-openapi.yml
- filename: spot-ai-locations-api-openapi.yml
  format: yaml
  label: Spot AI Locations API
  slug: spot-ai-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-locations-api-openapi.yml
- filename: spot-ai-lpi-api-openapi.yml
  format: yaml
  label: Spot AI LPI API
  slug: spot-ai-lpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-lpi-api-openapi.yml
- filename: spot-ai-lpr-api-openapi.yml
  format: yaml
  label: Spot AI LPR API
  slug: spot-ai-lpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-lpr-api-openapi.yml
- filename: spot-ai-shared-search-api-openapi.yml
  format: yaml
  label: Spot AI Shared Search API
  slug: spot-ai-shared-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-shared-search-api-openapi.yml
- filename: spot-ai-zones-api-openapi.yml
  format: yaml
  label: Spot AI Zones API
  slug: spot-ai-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-zones-api-openapi.yml
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
overview: 'Domain security posture for Spot AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spot AI
provider_slug: spot-ai
slug: spot-domain-security
source_filename: spot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-api.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:44:12 2026 GMT\n  hsts: null\ndomains:\n- domain: spot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/security/spot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Physical Security
- Surveillance
- Computer-Vision
- Artificial Intelligence
- Camera
- Analytics
- License Plate Recognition
- Webhook
- Integration
---
