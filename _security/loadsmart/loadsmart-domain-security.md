---
api_specs:
- filename: loadsmart-shipperguide-openapi.yml
  format: yaml
  label: Loadsmart ShipperGuide API
  slug: loadsmart-shipperguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/openapi/loadsmart-shipperguide-openapi.yml
- filename: loadsmart-opendock-openapi.yml
  format: yaml
  label: Opendock Nova (Neutron) API
  slug: loadsmart-opendock-nova-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/openapi/loadsmart-opendock-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loadsmart.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: loadsmart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: developer.loadsmart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: api.loadsmart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loadsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loadsmart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loadsmart
provider_slug: loadsmart
slug: loadsmart-domain-security
source_filename: loadsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loadsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: developer.loadsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.loadsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: loadsmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/security/loadsmart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Freight
- Logistics
- Transportation
- Supply Chain
- Digital Freight
- Freight Brokerage
- Truckload
- LTL
- Drayage
- Flatbed
- Multimodal
- TMS
- Dock Scheduling
- Yard Management
- Warehouse
- 4PL
- FreightTech
---
