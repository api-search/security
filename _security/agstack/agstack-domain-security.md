---
api_specs:
- filename: agstack-api-api-openapi.yml
  format: yaml
  label: AgStack Foundation api API
  slug: agstack-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-api-api-openapi.yml
- filename: agstack-auth-api-openapi.yml
  format: yaml
  label: AgStack Foundation Auth API
  slug: agstack-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-auth-api-openapi.yml
- filename: agstack-authentication-api-openapi.yml
  format: yaml
  label: AgStack Foundation Authentication API
  slug: agstack-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-authentication-api-openapi.yml
- filename: agstack-data-api-openapi.yml
  format: yaml
  label: AgStack Foundation Data API
  slug: agstack-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-data-api-openapi.yml
- filename: agstack-field-registration-post-api-openapi.yml
  format: yaml
  label: AgStack Foundation Field Registration (POST) API
  slug: agstack-field-registration-post-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-field-registration-post-api-openapi.yml
- filename: agstack-field-retrieval-queries-api-openapi.yml
  format: yaml
  label: AgStack Foundation Field Retrieval & Queries API
  slug: agstack-field-retrieval-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-field-retrieval-queries-api-openapi.yml
- filename: agstack-linkeddata-api-openapi.yml
  format: yaml
  label: AgStack Foundation Linkeddata API
  slug: agstack-linkeddata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-linkeddata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agstack.org
  spf: true
hosts:
- cert_expires: Sep 20 06:56:45 2026 GMT
  host: agstack.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 00:19:38 2026 GMT
  host: api-ar.agstack.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgStack Foundation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgStack Foundation
provider_slug: agstack
slug: agstack-domain-security
source_filename: agstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:56:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api-ar.agstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:19:38 2026 GMT\n  hsts: null\ndomains:\n- domain: agstack.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/security/agstack-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
---
