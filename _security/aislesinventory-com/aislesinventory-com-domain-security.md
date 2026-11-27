---
api_specs:
- filename: aislesinventory-com-agent-api-openapi.yml
  format: yaml
  label: Aisles Inc. Agent API
  slug: aislesinventory-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-agent-api-openapi.yml
- filename: aislesinventory-com-jobs-api-openapi.yml
  format: yaml
  label: Aisles Inc. Jobs API
  slug: aislesinventory-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-jobs-api-openapi.yml
- filename: aislesinventory-com-sandbox-api-openapi.yml
  format: yaml
  label: Aisles Inc. Sandbox API
  slug: aislesinventory-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-sandbox-api-openapi.yml
- filename: aislesinventory-com-search-api-openapi.yml
  format: yaml
  label: Aisles Inc. Search API
  slug: aislesinventory-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aislesinventory.com
  spf: false
hosts:
- cert_expires: Jan 14 19:41:21 2027 GMT
  host: aislesinventory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aisles Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aisles Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Aisles Inc.
provider_slug: aislesinventory-com
slug: aislesinventory-com-domain-security
source_filename: aislesinventory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aislesinventory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 19:41:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aislesinventory.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aislesinventory-com/security/aislesinventory-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Inventory
- Retail
- Stocks
- US
---
