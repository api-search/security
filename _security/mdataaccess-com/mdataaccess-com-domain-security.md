---
api_specs:
- filename: mdataaccess-com-discovery-api-openapi.yml
  format: yaml
  label: MDataAccess Discovery API
  slug: mdataaccess-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdataaccess-com/openapi/mdataaccess-com-discovery-api-openapi.yml
- filename: mdataaccess-com-enrichment-api-openapi.yml
  format: yaml
  label: MDataAccess Enrichment API
  slug: mdataaccess-com-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdataaccess-com/openapi/mdataaccess-com-enrichment-api-openapi.yml
- filename: mdataaccess-com-intelligence-api-openapi.yml
  format: yaml
  label: MDataAccess Intelligence API
  slug: mdataaccess-com-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdataaccess-com/openapi/mdataaccess-com-intelligence-api-openapi.yml
- filename: mdataaccess-com-system-api-openapi.yml
  format: yaml
  label: MDataAccess System API
  slug: mdataaccess-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdataaccess-com/openapi/mdataaccess-com-system-api-openapi.yml
- filename: mdataaccess-com-web-api-openapi.yml
  format: yaml
  label: MDataAccess Web API
  slug: mdataaccess-com-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdataaccess-com/openapi/mdataaccess-com-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mdataaccess.com
  spf: true
hosts:
- cert_expires: Dec 19 16:28:18 2026 GMT
  host: mdataaccess.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MDataAccess Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MDataAccess, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MDataAccess
provider_slug: mdataaccess-com
slug: mdataaccess-com-domain-security
source_filename: mdataaccess-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mdataaccess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 16:28:18 2026 GMT\n  hsts: null\ndomains:\n- domain: mdataaccess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mdataaccess-com/security/mdataaccess-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Data
- Business Intelligence
- Machine-native API
- Pay-per-request
---
