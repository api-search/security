---
api_specs:
- filename: serpresult-com-account-api-openapi.yml
  format: yaml
  label: serpresult-com Account API
  slug: serpresult-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-account-api-openapi.yml
- filename: serpresult-com-api-keys-api-openapi.yml
  format: yaml
  label: serpresult-com API keys API
  slug: serpresult-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-api-keys-api-openapi.yml
- filename: serpresult-com-billing-api-openapi.yml
  format: yaml
  label: serpresult-com Billing API
  slug: serpresult-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-billing-api-openapi.yml
- filename: serpresult-com-meta-api-openapi.yml
  format: yaml
  label: serpresult-com Meta API
  slug: serpresult-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-meta-api-openapi.yml
- filename: serpresult-com-search-api-openapi.yml
  format: yaml
  label: serpresult-com Search API
  slug: serpresult-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-search-api-openapi.yml
- filename: serpresult-com-usage-api-openapi.yml
  format: yaml
  label: serpresult-com Usage API
  slug: serpresult-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: serpresult.com
  spf: true
hosts:
- cert_expires: Dec 12 17:45:10 2026 GMT
  host: serpresult.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Serpresult Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for serpresult-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: serpresult-com
provider_slug: serpresult-com
slug: serpresult-com-domain-security
source_filename: serpresult-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serpresult.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 17:45:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: serpresult.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/serpresult-com/security/serpresult-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SERP
- Search
- API
- Aggregator
- SEO
---
