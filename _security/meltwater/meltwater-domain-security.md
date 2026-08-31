---
api_specs:
- filename: meltwater-account-management-api-openapi.yml
  format: yaml
  label: Meltwater Account Management API
  slug: meltwater-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-account-management-api-openapi.yml
- filename: meltwater-bring-your-own-content-byoc-api-openapi.yml
  format: yaml
  label: Meltwater Bring Your Own Content (BYOC) API
  slug: meltwater-bring-your-own-content-byoc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-bring-your-own-content-byoc-api-openapi.yml
- filename: meltwater-explore-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Analytics API
  slug: meltwater-explore-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-analytics-api-openapi.yml
- filename: meltwater-explore-assets-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Assets API
  slug: meltwater-explore-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-assets-api-openapi.yml
- filename: meltwater-explore-search-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Search API
  slug: meltwater-explore-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-search-api-openapi.yml
- filename: meltwater-listening-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Listening Analytics API
  slug: meltwater-listening-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-analytics-api-openapi.yml
- filename: meltwater-listening-exports-api-openapi.yml
  format: yaml
  label: Meltwater Listening Exports API
  slug: meltwater-listening-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-exports-api-openapi.yml
- filename: meltwater-listening-search-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search API
  slug: meltwater-listening-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-api-openapi.yml
- filename: meltwater-listening-search-management-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search Management API
  slug: meltwater-listening-search-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-management-api-openapi.yml
- filename: meltwater-listening-streaming-api-openapi.yml
  format: yaml
  label: Meltwater Listening Streaming API
  slug: meltwater-listening-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-streaming-api-openapi.yml
- filename: meltwater-mira-api-api-openapi.yml
  format: yaml
  label: Meltwater Mira API API
  slug: meltwater-mira-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-mira-api-api-openapi.yml
- filename: meltwater-owned-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Owned Analytics API
  slug: meltwater-owned-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-owned-analytics-api-openapi.yml
- filename: meltwater-analyze-api-openapi.yml
  format: yaml
  label: Meltwater Analyze API
  slug: meltwater-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-analyze-api-openapi.yml
- filename: meltwater-export-api-openapi.yml
  format: yaml
  label: Meltwater Export API
  slug: meltwater-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-export-api-openapi.yml
- filename: meltwater-llm-api-openapi.yml
  format: yaml
  label: Meltwater LLM API
  slug: meltwater-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-llm-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meltwater.com
  spf: true
hosts:
- cert_expires: Oct 30 16:31:36 2026 GMT
  host: www.meltwater.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: developer.meltwater.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.meltwater.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Meltwater Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meltwater, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meltwater
provider_slug: meltwater
slug: meltwater-domain-security
source_filename: meltwater-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meltwater.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 16:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.meltwater.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.meltwater.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: meltwater.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/security/meltwater-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media Monitoring
- Social Listening
- PR Analytics
- Brand Intelligence
- News API
- Social Analytics
- Media Intelligence
---
