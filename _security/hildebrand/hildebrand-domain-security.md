---
api_specs:
- filename: hildebrand-glowmarkt-user-system-swagger.json
  format: json
  label: Glowmarkt User System API
  slug: glowmarkt-user-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-user-system-swagger.json
- filename: hildebrand-glowmarkt-resource-system-swagger.json
  format: json
  label: Glowmarkt Resource System API
  slug: glowmarkt-resource-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-resource-system-swagger.json
- filename: hildebrand-glowmarkt-virtual-entity-system-swagger.json
  format: json
  label: Glowmarkt Virtual Entity System API
  slug: glowmarkt-virtual-entity-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json
- filename: hildebrand-glowmarkt-device-management-system-swagger.json
  format: json
  label: Glowmarkt Device Management System API
  slug: glowmarkt-device-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-device-management-system-swagger.json
- filename: hildebrand-glowmarkt-notification-system-swagger.json
  format: json
  label: Glowmarkt Notification System API
  slug: glowmarkt-notification-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-notification-system-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hildebrand.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glowmarkt.com
  spf: true
hosts:
- cert_expires: Oct 21 02:52:36 2026 GMT
  host: www.hildebrand.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 05:20:18 2026 GMT
  host: api.glowmarkt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hildebrand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hildebrand, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hildebrand
provider_slug: hildebrand
slug: hildebrand-domain-security
source_filename: hildebrand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hildebrand.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:52:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.glowmarkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:20:18 2026 GMT\n  hsts: null\ndomains:\n- domain: hildebrand.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: glowmarkt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/security/hildebrand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Data
- Demand Response
- IoT
- Metering
---
