---
api_specs:
- filename: actian-access-tokens-api-openapi.yml
  format: yaml
  label: Actian Corporation Access Tokens API
  slug: actian-access-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-access-tokens-api-openapi.yml
- filename: actian-admin-user-api-openapi.yml
  format: yaml
  label: Actian Corporation Admin User API
  slug: actian-admin-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-admin-user-api-openapi.yml
- filename: actian-collections-api-openapi.yml
  format: yaml
  label: Actian Corporation Collections API
  slug: actian-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-collections-api-openapi.yml
- filename: actian-count-api-openapi.yml
  format: yaml
  label: Actian Corporation Count API
  slug: actian-count-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-count-api-openapi.yml
- filename: actian-filters-api-openapi.yml
  format: yaml
  label: Actian Corporation Filters API
  slug: actian-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-filters-api-openapi.yml
- filename: actian-points-api-openapi.yml
  format: yaml
  label: Actian Corporation Points API
  slug: actian-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-points-api-openapi.yml
- filename: actian-scroll-api-openapi.yml
  format: yaml
  label: Actian Corporation Scroll API
  slug: actian-scroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-scroll-api-openapi.yml
- filename: actian-search-api-openapi.yml
  format: yaml
  label: Actian Corporation Search API
  slug: actian-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: actian.com
  spf: true
hosts:
- cert_expires: Jan 15 02:48:54 2027 GMT
  host: actian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Actian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actian Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Actian Corporation
provider_slug: actian
slug: actian-domain-security
source_filename: actian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 02:48:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: actian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/actian/security/actian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Integration
- Analytics
- Artificial Intelligence
- Enterprise
---
