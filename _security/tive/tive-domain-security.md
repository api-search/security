---
api_specs:
- filename: tive-openapi.yml
  format: yaml
  label: Tive Shipments API
  slug: tive-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Trackers / Devices API
  slug: tive-trackers-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Sensor Data API
  slug: tive-sensor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Alerts API
  slug: tive-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Webhooks API
  slug: tive-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tive.com
  spf: true
hosts:
- cert_expires: Aug 16 07:05:06 2026 GMT
  host: www.tive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:29:32 2026 GMT
  host: developers.tive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.tive.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tive
provider_slug: tive
slug: tive-domain-security
source_filename: tive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:05:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.tive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:29:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tive.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/security/tive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Shipment Visibility
- Logistics
- IoT
- Trackers
- Real Time
---
