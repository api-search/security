---
api_specs:
- filename: gaplessly-com-agent-mcp-api-openapi.yml
  format: yaml
  label: Gaplessly Agent (MCP) API
  slug: gaplessly-com-agent-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-agent-mcp-api-openapi.yml
- filename: gaplessly-com-appointments-engine-api-openapi.yml
  format: yaml
  label: Gaplessly Appointments engine API
  slug: gaplessly-com-appointments-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-appointments-engine-api-openapi.yml
- filename: gaplessly-com-guest-self-service-api-openapi.yml
  format: yaml
  label: Gaplessly Guest self-service API
  slug: gaplessly-com-guest-self-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-guest-self-service-api-openapi.yml
- filename: gaplessly-com-hospitality-engine-api-openapi.yml
  format: yaml
  label: Gaplessly Hospitality engine API
  slug: gaplessly-com-hospitality-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-hospitality-engine-api-openapi.yml
- filename: gaplessly-com-public-booking-appointments-api-openapi.yml
  format: yaml
  label: Gaplessly Public booking (appointments) API
  slug: gaplessly-com-public-booking-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-public-booking-appointments-api-openapi.yml
- filename: gaplessly-com-public-booking-hospitality-api-openapi.yml
  format: yaml
  label: Gaplessly Public booking (hospitality) API
  slug: gaplessly-com-public-booking-hospitality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-public-booking-hospitality-api-openapi.yml
- filename: gaplessly-com-shared-api-openapi.yml
  format: yaml
  label: Gaplessly Shared API
  slug: gaplessly-com-shared-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-shared-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gaplessly.com
  spf: true
hosts:
- cert_expires: Feb  3 12:51:09 2027 GMT
  host: gaplessly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gaplessly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gaplessly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gaplessly
provider_slug: gaplessly-com
slug: gaplessly-com-domain-security
source_filename: gaplessly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gaplessly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 12:51:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gaplessly.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gaplessly-com/security/gaplessly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Booking
- Software-as-a-Service
- Restaurant
- Scheduling
---
