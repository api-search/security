---
api_specs:
- filename: legivel-com-health-api-openapi.yml
  format: yaml
  label: legivel Health API
  slug: legivel-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-health-api-openapi.yml
- filename: legivel-com-openapi-json-api-openapi.yml
  format: yaml
  label: legivel Openapi.json API
  slug: legivel-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-openapi-json-api-openapi.yml
- filename: legivel-com-render-api-openapi.yml
  format: yaml
  label: legivel Render API
  slug: legivel-com-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-render-api-openapi.yml
- filename: legivel-com-templates-api-openapi.yml
  format: yaml
  label: legivel Templates API
  slug: legivel-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-templates-api-openapi.yml
- filename: legivel-com-usage-api-openapi.yml
  format: yaml
  label: legivel Usage API
  slug: legivel-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: legivel.com
  spf: true
hosts:
- cert_expires: Jan  9 18:07:24 2027 GMT
  host: legivel.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 18:07:24 2027 GMT
  host: api.legivel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: legivel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for legivel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: legivel
provider_slug: legivel-com
slug: legivel-com-domain-security
source_filename: legivel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: legivel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:07:24 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.legivel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:07:24 2027 GMT\n  hsts: null\ndomains:\n- domain: legivel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/legivel-com/security/legivel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Markdown
- PDF
- Conversion
- Software-as-a-Service
---
