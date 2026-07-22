---
api_specs:
- filename: servicechannel-service-automation-openapi-original.json
  format: json
  label: ServiceChannel Service Automation API
  slug: servicechannel-service-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-service-automation-openapi-original.json
- filename: servicechannel-fixxbook-openapi-original.json
  format: json
  label: ServiceChannel Fixxbook API
  slug: servicechannel-fixxbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-fixxbook-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: servicechannel.com
  spf: true
hosts:
- cert_expires: Jul 25 23:59:59 2026 GMT
  host: www.servicechannel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 25 23:59:59 2026 GMT
  host: sb2fixxbook.servicechannel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 25 23:59:59 2026 GMT
  host: sb2api.servicechannel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servicechannel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ServiceChannel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ServiceChannel
provider_slug: servicechannel
slug: servicechannel-domain-security
source_filename: servicechannel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.servicechannel.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sb2fixxbook.servicechannel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sb2api.servicechannel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: servicechannel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/security/servicechannel-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Services
- Facilities Management
- Work Orders
- Field Service
- Maintenance
- Asset Management
- Service Providers
- Invoicing
---
