---
api_specs:
- filename: locus-sh-homebasemaster-api-openapi.yml
  format: yaml
  label: Locus HomebaseMaster API
  slug: locus-sh-homebasemaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-homebasemaster-api-openapi.yml
- filename: locus-sh-locationmaster-api-openapi.yml
  format: yaml
  label: Locus LocationMaster API
  slug: locus-sh-locationmaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-locationmaster-api-openapi.yml
- filename: locus-sh-order-api-openapi.yml
  format: yaml
  label: Locus Order API
  slug: locus-sh-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-order-api-openapi.yml
- filename: locus-sh-orderserviceability-api-openapi.yml
  format: yaml
  label: Locus OrderServiceability API
  slug: locus-sh-orderserviceability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-orderserviceability-api-openapi.yml
- filename: locus-sh-personnelmaster-api-openapi.yml
  format: yaml
  label: Locus PersonnelMaster API
  slug: locus-sh-personnelmaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-personnelmaster-api-openapi.yml
- filename: locus-sh-rider-api-openapi.yml
  format: yaml
  label: Locus Rider API
  slug: locus-sh-rider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-rider-api-openapi.yml
- filename: locus-sh-riderpersona-api-openapi.yml
  format: yaml
  label: Locus RiderPersona API
  slug: locus-sh-riderpersona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-riderpersona-api-openapi.yml
- filename: locus-sh-roster-api-openapi.yml
  format: yaml
  label: Locus Roster API
  slug: locus-sh-roster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-roster-api-openapi.yml
- filename: locus-sh-servicetype-api-openapi.yml
  format: yaml
  label: Locus ServiceType API
  slug: locus-sh-servicetype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-servicetype-api-openapi.yml
- filename: locus-sh-servicetypeconfiguration-api-openapi.yml
  format: yaml
  label: Locus ServiceTypeConfiguration API
  slug: locus-sh-servicetypeconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-servicetypeconfiguration-api-openapi.yml
- filename: locus-sh-shifttag-api-openapi.yml
  format: yaml
  label: Locus ShiftTag API
  slug: locus-sh-shifttag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-shifttag-api-openapi.yml
- filename: locus-sh-skumaster-api-openapi.yml
  format: yaml
  label: Locus SKUMaster API
  slug: locus-sh-skumaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-skumaster-api-openapi.yml
- filename: locus-sh-teammaster-api-openapi.yml
  format: yaml
  label: Locus TeamMaster API
  slug: locus-sh-teammaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-teammaster-api-openapi.yml
- filename: locus-sh-transporter-api-openapi.yml
  format: yaml
  label: Locus Transporter API
  slug: locus-sh-transporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-transporter-api-openapi.yml
- filename: locus-sh-vehicle-api-openapi.yml
  format: yaml
  label: Locus Vehicle API
  slug: locus-sh-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-vehicle-api-openapi.yml
- filename: locus-sh-vehiclemodel-api-openapi.yml
  format: yaml
  label: Locus VehicleModel API
  slug: locus-sh-vehiclemodel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-sh-vehiclemodel-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locus.sh
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: locus-api.com
  spf: false
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: locus.sh
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: docs.locus.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: oms.locus-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Locus Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Locus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Locus
provider_slug: locus-sh
slug: locus-sh-domain-security
source_filename: locus-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: locus.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.locus.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\n- host: oms.locus-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: locus.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: locus-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/security/locus-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Last Mile Delivery
- Route Optimization
- Dispatch Planning
- Transportation Management
- Fleet Management
- Supply Chain
- Order Management
- Fulfillment
- Track and Trace
- Retail
- E-Commerce
- Artificial Intelligence
- India
---
