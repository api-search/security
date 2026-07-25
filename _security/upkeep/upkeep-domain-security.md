---
api_specs:
- filename: upkeep-assets-api-openapi.yml
  format: yaml
  label: UpKeep Assets API
  slug: upkeep-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-assets-api-openapi.yml
- filename: upkeep-authentication-api-openapi.yml
  format: yaml
  label: UpKeep Authentication API
  slug: upkeep-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-authentication-api-openapi.yml
- filename: upkeep-locations-api-openapi.yml
  format: yaml
  label: UpKeep Locations API
  slug: upkeep-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-locations-api-openapi.yml
- filename: upkeep-meters-api-openapi.yml
  format: yaml
  label: UpKeep Meters API
  slug: upkeep-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-meters-api-openapi.yml
- filename: upkeep-parts-api-openapi.yml
  format: yaml
  label: UpKeep Parts API
  slug: upkeep-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-parts-api-openapi.yml
- filename: upkeep-preventive-maintenance-api-openapi.yml
  format: yaml
  label: UpKeep Preventive Maintenance API
  slug: upkeep-preventive-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-preventive-maintenance-api-openapi.yml
- filename: upkeep-purchase-orders-api-openapi.yml
  format: yaml
  label: UpKeep Purchase Orders API
  slug: upkeep-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-purchase-orders-api-openapi.yml
- filename: upkeep-requests-api-openapi.yml
  format: yaml
  label: UpKeep Requests API
  slug: upkeep-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-requests-api-openapi.yml
- filename: upkeep-webhooks-api-openapi.yml
  format: yaml
  label: UpKeep Webhooks API
  slug: upkeep-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-webhooks-api-openapi.yml
- filename: upkeep-work-orders-api-openapi.yml
  format: yaml
  label: UpKeep Work Orders API
  slug: upkeep-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-work-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: upkeep.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onupkeep.com
  spf: true
hosts:
- cert_expires: Aug 20 04:44:00 2026 GMT
  host: upkeep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: developers.onupkeep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:22 2026 GMT
  host: api.onupkeep.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upkeep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UpKeep, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: UpKeep
provider_slug: upkeep
slug: upkeep-domain-security
source_filename: upkeep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:44:00 2026 GMT\n  hsts: false\n- host: developers.onupkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.onupkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:22 2026 GMT\n  hsts: null\ndomains:\n- domain: upkeep.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: onupkeep.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/security/upkeep-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- CMMS
- Maintenance Management
- Asset Management
- Facility Management
- Work Orders
---
