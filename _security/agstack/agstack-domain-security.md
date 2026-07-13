---
api_specs:
- filename: agstack-openagri-weather-service-openapi.yml
  format: yaml
  label: OpenAgri Weather Service
  slug: openagri-weather-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-openagri-weather-service-openapi.yml
- filename: agstack-openagri-farm-calendar-openapi.yml
  format: yaml
  label: OpenAgri Farm Calendar
  slug: openagri-farm-calendar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-openagri-farm-calendar-openapi.yml
- filename: agstack-asset-registry-openapi.yml
  format: yaml
  label: AgStack Asset Registry
  slug: asset-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-asset-registry-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agstack.org
  spf: true
hosts:
- cert_expires: Sep 20 06:56:45 2026 GMT
  host: agstack.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 00:19:38 2026 GMT
  host: api-ar.agstack.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgStack Foundation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgStack Foundation
provider_slug: agstack
slug: agstack-domain-security
source_filename: agstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:56:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api-ar.agstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:19:38 2026 GMT\n  hsts: null\ndomains:\n- domain: agstack.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/security/agstack-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
---
