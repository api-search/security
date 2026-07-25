---
api_specs:
- filename: herald-applications-api-openapi.yml
  format: yaml
  label: Herald Applications API
  slug: herald-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-applications-api-openapi.yml
- filename: herald-authentication-api-openapi.yml
  format: yaml
  label: Herald Authentication API
  slug: herald-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-authentication-api-openapi.yml
- filename: herald-classifications-api-openapi.yml
  format: yaml
  label: Herald Classifications API
  slug: herald-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-classifications-api-openapi.yml
- filename: herald-distributors-api-openapi.yml
  format: yaml
  label: Herald Distributors API
  slug: herald-distributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-distributors-api-openapi.yml
- filename: herald-files-api-openapi.yml
  format: yaml
  label: Herald Files API
  slug: herald-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-files-api-openapi.yml
- filename: herald-producers-api-openapi.yml
  format: yaml
  label: Herald Producers API
  slug: herald-producers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-producers-api-openapi.yml
- filename: herald-products-api-openapi.yml
  format: yaml
  label: Herald Products API
  slug: herald-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-products-api-openapi.yml
- filename: herald-quotes-api-openapi.yml
  format: yaml
  label: Herald Quotes API
  slug: herald-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-quotes-api-openapi.yml
- filename: herald-submissions-api-openapi.yml
  format: yaml
  label: Herald Submissions API
  slug: herald-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-submissions-api-openapi.yml
- filename: herald-webhooks-api-openapi.yml
  format: yaml
  label: Herald Webhooks API
  slug: herald-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/openapi/herald-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heraldapi.com
  spf: true
hosts:
- cert_expires: Sep 29 15:45:04 2026 GMT
  host: www.heraldapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:16:47 2026 GMT
  host: docs.heraldapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.heraldapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Herald Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Herald, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Herald
provider_slug: herald
slug: herald-domain-security
source_filename: herald-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heraldapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:45:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.heraldapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.heraldapi.com\n  https: false\ndomains:\n- domain: heraldapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herald/refs/heads/main/security/herald-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Commercial Insurance
- Quoting
- Carriers
---
