---
api_specs:
- filename: shipwell-carriers-api-openapi.yml
  format: yaml
  label: Shipwell Carriers API
  slug: shipwell-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-carriers-api-openapi.yml
- filename: shipwell-events-and-webhooks-api-openapi.yml
  format: yaml
  label: Shipwell Events and Webhooks API
  slug: shipwell-events-and-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-events-and-webhooks-api-openapi.yml
- filename: shipwell-orders-api-openapi.yml
  format: yaml
  label: Shipwell Orders API
  slug: shipwell-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-orders-api-openapi.yml
- filename: shipwell-quoting-api-openapi.yml
  format: yaml
  label: Shipwell Quoting API
  slug: shipwell-quoting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-quoting-api-openapi.yml
- filename: shipwell-shipments-api-openapi.yml
  format: yaml
  label: Shipwell Shipments API
  slug: shipwell-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/openapi/shipwell-shipments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipwell.com
  spf: true
hosts:
- cert_expires: Sep 10 05:11:36 2026 GMT
  host: www.shipwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 03:34:25 2026 GMT
  host: docs.shipwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 21:50:30 2026 GMT
  host: api.shipwell.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipwell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shipwell
provider_slug: shipwell
slug: shipwell-domain-security
source_filename: shipwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.shipwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 03:34:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shipwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:50:30 2026 GMT\n  hsts: false\ndomains:\n- domain: shipwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipwell/refs/heads/main/security/shipwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation Management
- TMS
- Freight
- Logistics
- Shipping
- Supply Chain
---
