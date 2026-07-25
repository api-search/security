---
api_specs:
- filename: dassault-accreditations-api-openapi.yml
  format: yaml
  label: Dassault Systèmes accreditations API
  slug: dassault-accreditations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-accreditations-api-openapi.yml
- filename: dassault-apikeys-api-openapi.yml
  format: yaml
  label: Dassault Systèmes apikeys API
  slug: dassault-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-apikeys-api-openapi.yml
- filename: dassault-leads-opportunities-api-openapi.yml
  format: yaml
  label: Dassault Systèmes leads-opportunities API
  slug: dassault-leads-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-leads-opportunities-api-openapi.yml
- filename: dassault-orders-api-openapi.yml
  format: yaml
  label: Dassault Systèmes orders API
  slug: dassault-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-orders-api-openapi.yml
- filename: dassault-portfolio-items-api-openapi.yml
  format: yaml
  label: Dassault Systèmes portfolio-items API
  slug: dassault-portfolio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-portfolio-items-api-openapi.yml
- filename: dassault-price-lists-api-openapi.yml
  format: yaml
  label: Dassault Systèmes price-lists API
  slug: dassault-price-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-price-lists-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 3ds.com
  spf: true
hosts:
- cert_expires: Sep  5 20:33:46 2026 GMT
  host: www.3ds.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 21:35:48 2026 GMT
  host: apigw-prd.3ds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 22:17:35 2026 GMT
  host: partners.3ds.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dassault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dassault Systèmes, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dassault Systèmes
provider_slug: dassault
slug: dassault-domain-security
source_filename: dassault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3ds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: apigw-prd.3ds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:35:48 2026 GMT\n  hsts: null\n- host: partners.3ds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: 3ds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/security/dassault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3DEXPERIENCE
- PLM
- Product Lifecycle Management
- CAD
- Manufacturing
- SolidWorks
- CATIA
- ENOVIA
- Engineering
- 3D Collaboration
---
