---
api_specs:
- filename: budbee-box-api-openapi.yml
  format: yaml
  label: Budbee Box API
  slug: budbee-box-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-box-api-openapi.yml
- filename: budbee-boxes-api-openapi.yml
  format: yaml
  label: Budbee Boxes API
  slug: budbee-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-boxes-api-openapi.yml
- filename: budbee-budbee-api-api-openapi.yml
  format: yaml
  label: Budbee Budbee API
  slug: budbee-budbee-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-budbee-api-api-openapi.yml
- filename: budbee-intervals-api-openapi.yml
  format: yaml
  label: Budbee Intervals API
  slug: budbee-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-intervals-api-openapi.yml
- filename: budbee-multiple-api-openapi.yml
  format: yaml
  label: Budbee Multiple API
  slug: budbee-multiple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-multiple-api-openapi.yml
- filename: budbee-postalcodes-api-openapi.yml
  format: yaml
  label: Budbee Postalcodes API
  slug: budbee-postalcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-postalcodes-api-openapi.yml
- filename: budbee-returns-api-openapi.yml
  format: yaml
  label: Budbee Returns API
  slug: budbee-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-returns-api-openapi.yml
- filename: budbee-users-api-openapi.yml
  format: yaml
  label: Budbee Users API
  slug: budbee-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-users-api-openapi.yml
- filename: budbee-webhooks-api-openapi.yml
  format: yaml
  label: Budbee Webhooks API
  slug: budbee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/openapi/budbee-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hiive.com
  spf: true
hosts:
- cert_expires: Dec 14 14:19:32 2026 GMT
  host: www.hiive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Budbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Budbee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Budbee
provider_slug: budbee
slug: budbee-domain-security
source_filename: budbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hiive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 14:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hiive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/budbee/refs/heads/main/security/budbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Delivery
- Logistics
- E-Commerce
- Sustainability
---
