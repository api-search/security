---
api_specs:
- filename: apimatic-apis-api-openapi.yml
  format: yaml
  label: APIMatic APIs API
  slug: apimatic-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-apis-api-openapi.yml
- filename: apimatic-portals-api-openapi.yml
  format: yaml
  label: APIMatic Portals API
  slug: apimatic-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-portals-api-openapi.yml
- filename: apimatic-sdk-generation-api-openapi.yml
  format: yaml
  label: APIMatic SDK Generation API
  slug: apimatic-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-sdk-generation-api-openapi.yml
- filename: apimatic-transformation-api-openapi.yml
  format: yaml
  label: APIMatic Transformation API
  slug: apimatic-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-transformation-api-openapi.yml
- filename: apimatic-validation-api-openapi.yml
  format: yaml
  label: APIMatic Validation API
  slug: apimatic-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apimatic.io
  spf: true
hosts:
- cert_expires: Sep 23 02:04:05 2026 GMT
  host: www.apimatic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:25:08 2026 GMT
  host: docs.apimatic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.apimatic.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apimatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIMatic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: APIMatic
provider_slug: apimatic
slug: apimatic-domain-security
source_filename: apimatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apimatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:04:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.apimatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:25:08 2026 GMT\n  hsts: false\n- host: api.apimatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apimatic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/security/apimatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
---
