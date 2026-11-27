---
api_specs:
- filename: interzoid-com-data-enhancement-api-openapi.yml
  format: yaml
  label: Interzoid Data Enhancement API
  slug: interzoid-com-data-enhancement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-enhancement-api-openapi.yml
- filename: interzoid-com-data-enrichment-api-openapi.yml
  format: yaml
  label: Interzoid Data Enrichment API
  slug: interzoid-com-data-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-enrichment-api-openapi.yml
- filename: interzoid-com-data-matching-api-openapi.yml
  format: yaml
  label: Interzoid Data Matching API
  slug: interzoid-com-data-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-matching-api-openapi.yml
- filename: interzoid-com-data-standardization-api-openapi.yml
  format: yaml
  label: Interzoid Data Standardization API
  slug: interzoid-com-data-standardization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-standardization-api-openapi.yml
- filename: interzoid-com-utility-api-openapi.yml
  format: yaml
  label: Interzoid Utility API
  slug: interzoid-com-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: interzoid.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: interzoid.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Interzoid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interzoid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Interzoid
provider_slug: interzoid-com
slug: interzoid-com-domain-security
source_filename: interzoid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: interzoid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: interzoid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/interzoid-com/security/interzoid-com-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Data
- Data Enrichment
- Matching
- Business Intelligence
---
