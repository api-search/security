---
api_specs:
- filename: ploid-account-api-openapi.yml
  format: yaml
  label: Ploid Account API
  slug: ploid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-account-api-openapi.yml
- filename: ploid-discovery-api-openapi.yml
  format: yaml
  label: Ploid Discovery API
  slug: ploid-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-discovery-api-openapi.yml
- filename: ploid-enrichment-api-openapi.yml
  format: yaml
  label: Ploid Enrichment API
  slug: ploid-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-enrichment-api-openapi.yml
- filename: ploid-harness-api-openapi.yml
  format: yaml
  label: Ploid Harness API
  slug: ploid-harness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-harness-api-openapi.yml
- filename: ploid-monitors-api-openapi.yml
  format: yaml
  label: Ploid Monitors API
  slug: ploid-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-monitors-api-openapi.yml
- filename: ploid-people-api-openapi.yml
  format: yaml
  label: Ploid People API
  slug: ploid-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-people-api-openapi.yml
- filename: ploid-search-api-openapi.yml
  format: yaml
  label: Ploid Search API
  slug: ploid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-search-api-openapi.yml
- filename: ploid-social-api-openapi.yml
  format: yaml
  label: Ploid Social API
  slug: ploid-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-social-api-openapi.yml
- filename: ploid-linked-in-api-openapi.yml
  format: yaml
  label: Ploid Linked In API
  slug: ploid-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-linked-in-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ploid.com
  spf: true
hosts:
- cert_expires: Dec 19 05:10:24 2026 GMT
  host: ploid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ploid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ploid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ploid
provider_slug: ploid
slug: ploid-domain-security
source_filename: ploid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ploid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 05:10:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ploid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/security/ploid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- People Data
- People Search
- Contact Enrichment
- Sales Intelligence
- Recruiting
- LinkedIn
- MCP
- Agents
- Data Enrichment
---
