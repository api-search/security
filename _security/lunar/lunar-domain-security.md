---
api_specs:
- filename: lunar-configuration-api-openapi.yml
  format: yaml
  label: Lunar Configuration API
  slug: lunar-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-configuration-api-openapi.yml
- filename: lunar-discovery-api-openapi.yml
  format: yaml
  label: Lunar Discovery API
  slug: lunar-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-discovery-api-openapi.yml
- filename: lunar-doctor-api-openapi.yml
  format: yaml
  label: Lunar Doctor API
  slug: lunar-doctor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-doctor-api-openapi.yml
- filename: lunar-flows-api-openapi.yml
  format: yaml
  label: Lunar Flows API
  slug: lunar-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-flows-api-openapi.yml
- filename: lunar-handshake-api-openapi.yml
  format: yaml
  label: Lunar Handshake API
  slug: lunar-handshake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-handshake-api-openapi.yml
- filename: lunar-policies-api-openapi.yml
  format: yaml
  label: Lunar Policies API
  slug: lunar-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-policies-api-openapi.yml
- filename: lunar-health-api-openapi.yml
  format: yaml
  label: Lunar Health API
  slug: lunar-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-health-api-openapi.yml
- filename: lunar-proxy-api-openapi.yml
  format: yaml
  label: Lunar Proxy API
  slug: lunar-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/openapi/lunar-proxy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunar.dev
  spf: true
hosts:
- cert_expires: Sep  3 20:09:20 2026 GMT
  host: www.lunar.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 05:01:00 2026 GMT
  host: docs.lunar.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 13:32:26 2026 GMT
  host: app.lunar.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lunar
provider_slug: lunar
slug: lunar-domain-security
source_filename: lunar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lunar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:09:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lunar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:01:00 2026 GMT\n  hsts: false\n- host: app.lunar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 13:32:26 2026 GMT\n  hsts: false\ndomains:\n- domain: lunar.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar/refs/heads/main/security/lunar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- API Gateway
- AI Gateway
- MCP Gateway
- Rate Limiting
- Quota Enforcement
- API Monetization
- Traffic Management
- API Governance
- Cost Controls
- Observability
---
