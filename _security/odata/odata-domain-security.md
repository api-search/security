---
api_specs:
- filename: odata-batch-api-openapi.yml
  format: yaml
  label: OData $Batch API
  slug: odata-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odata/openapi/odata-batch-api-openapi.yml
- filename: odata-metadata-api-openapi.yml
  format: yaml
  label: OData $Metadata API
  slug: odata-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odata/openapi/odata-metadata-api-openapi.yml
- filename: odata-odata-service-api-api-openapi.yml
  format: yaml
  label: OData Service API
  slug: odata-odata-service-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odata/openapi/odata-odata-service-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: odata.org
  spf: false
hosts:
- cert_expires: Jan 21 20:06:15 2027 GMT
  host: www.odata.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 20:06:15 2027 GMT
  host: services.odata.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: OData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OData, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OData
provider_slug: odata
slug: odata-domain-security
source_filename: odata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:06:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.odata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:06:15 2027 GMT\n  hsts: false\ndomains:\n- domain: odata.org\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/odata/security/odata-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- OASIS Standard
- OData
- Open Data Protocol
- Query Language
- RESTful APIs
---
