---
api_specs:
- filename: rendlet-com-checkout-api-openapi.yml
  format: yaml
  label: rendlet-com Checkout API
  slug: rendlet-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-checkout-api-openapi.yml
- filename: rendlet-com-pdf-api-openapi.yml
  format: yaml
  label: rendlet-com PDF API
  slug: rendlet-com-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-pdf-api-openapi.yml
- filename: rendlet-com-signup-api-openapi.yml
  format: yaml
  label: rendlet-com Signup API
  slug: rendlet-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-signup-api-openapi.yml
- filename: rendlet-com-templates-api-openapi.yml
  format: yaml
  label: rendlet-com Templates API
  slug: rendlet-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-templates-api-openapi.yml
- filename: rendlet-com-usage-api-openapi.yml
  format: yaml
  label: rendlet-com Usage API
  slug: rendlet-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rendlet.com
  spf: true
hosts:
- cert_expires: Jan 15 23:03:22 2027 GMT
  host: rendlet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rendlet Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rendlet-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: rendlet-com
provider_slug: rendlet-com
slug: rendlet-com-domain-security
source_filename: rendlet-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rendlet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:03:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rendlet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rendlet-com/security/rendlet-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PDF
- API
- DocumentGeneration
- SaaS
- DeveloperFriendly
- AI
---
