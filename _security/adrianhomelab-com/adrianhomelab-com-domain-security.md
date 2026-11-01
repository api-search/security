---
api_specs:
- filename: adrianhomelab-com-billing-api-openapi.yml
  format: yaml
  label: adrianhomelab-com Billing API
  slug: adrianhomelab-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrianhomelab-com/openapi/adrianhomelab-com-billing-api-openapi.yml
- filename: adrianhomelab-com-lookups-api-openapi.yml
  format: yaml
  label: adrianhomelab-com Lookups API
  slug: adrianhomelab-com-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrianhomelab-com/openapi/adrianhomelab-com-lookups-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adrianhomelab.com
  spf: true
hosts:
- cert_expires: Dec 27 06:17:16 2026 GMT
  host: adrianhomelab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adrianhomelab Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adrianhomelab-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: adrianhomelab-com
provider_slug: adrianhomelab-com
slug: adrianhomelab-com-domain-security
source_filename: adrianhomelab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adrianhomelab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 06:17:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adrianhomelab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adrianhomelab-com/security/adrianhomelab-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- frontend
- react
- javascript
- typescript
- web-development
- portfolio
---
