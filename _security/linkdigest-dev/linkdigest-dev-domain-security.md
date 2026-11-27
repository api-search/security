---
api_specs:
- filename: linkdigest-dev-capture-api-openapi.yml
  format: yaml
  label: LinkDigest Capture API
  slug: linkdigest-dev-capture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-capture-api-openapi.yml
- filename: linkdigest-dev-digest-api-openapi.yml
  format: yaml
  label: LinkDigest Digest API
  slug: linkdigest-dev-digest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-digest-api-openapi.yml
- filename: linkdigest-dev-health-api-openapi.yml
  format: yaml
  label: LinkDigest Health API
  slug: linkdigest-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-health-api-openapi.yml
- filename: linkdigest-dev-keys-api-openapi.yml
  format: yaml
  label: LinkDigest Keys API
  slug: linkdigest-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-keys-api-openapi.yml
- filename: linkdigest-dev-radar-api-openapi.yml
  format: yaml
  label: LinkDigest Radar API
  slug: linkdigest-dev-radar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-radar-api-openapi.yml
- filename: linkdigest-dev-search-api-openapi.yml
  format: yaml
  label: LinkDigest Search API
  slug: linkdigest-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-search-api-openapi.yml
- filename: linkdigest-dev-usage-api-openapi.yml
  format: yaml
  label: LinkDigest Usage API
  slug: linkdigest-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-usage-api-openapi.yml
- filename: linkdigest-dev-watch-api-openapi.yml
  format: yaml
  label: LinkDigest Watch API
  slug: linkdigest-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linkdigest.dev
  spf: true
hosts:
- cert_expires: Mar 11 14:49:43 2027 GMT
  host: linkdigest.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LinkDigest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkDigest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LinkDigest
provider_slug: linkdigest-dev
slug: linkdigest-dev-domain-security
source_filename: linkdigest-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkdigest.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 14:49:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linkdigest.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/linkdigest-dev/security/linkdigest-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Social Media
- Data Extraction
- Search
- Content Aggregation
---
