---
api_specs:
- filename: jaggaer-aso-ches-openapi.yml
  format: yaml
  label: JAGGAER ASO Customer Host Entity Service API
  slug: jaggaer-aso-customer-host-entity-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-aso-ches-openapi.yml
- filename: jaggaer-aso-ees-openapi.yml
  format: yaml
  label: JAGGAER ASO Event Entity Service API
  slug: jaggaer-aso-event-entity-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-aso-ees-openapi.yml
- filename: jaggaer-aso-quay-openapi.yml
  format: yaml
  label: JAGGAER ASO Quay Optimization API
  slug: jaggaer-aso-quay-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-aso-quay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jaggaer.com
  spf: true
hosts:
- cert_expires: Aug 12 02:41:01 2026 GMT
  host: www.jaggaer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: asodocs.jaggaer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: ches.aso-api.jaggaer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jaggaer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAGGAER, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: JAGGAER
provider_slug: jaggaer
slug: jaggaer-domain-security
source_filename: jaggaer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: asodocs.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ches.aso-api.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jaggaer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/security/jaggaer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Procurement
- Sourcing
- Supplier Management
- Contracts
- Spend Analytics
- eProcurement
- Source-to-Pay
- Procure-to-Pay
---
