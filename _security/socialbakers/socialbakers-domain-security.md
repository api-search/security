---
api_specs:
- filename: socialbakers-ads-api-openapi.yml
  format: yaml
  label: Socialbakers Ads API
  slug: socialbakers-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-ads-api-openapi.yml
- filename: socialbakers-assets-api-openapi.yml
  format: yaml
  label: Socialbakers Assets API
  slug: socialbakers-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-assets-api-openapi.yml
- filename: socialbakers-care-api-openapi.yml
  format: yaml
  label: Socialbakers Care API
  slug: socialbakers-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-care-api-openapi.yml
- filename: socialbakers-community-api-openapi.yml
  format: yaml
  label: Socialbakers Community API
  slug: socialbakers-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-community-api-openapi.yml
- filename: socialbakers-listening-api-openapi.yml
  format: yaml
  label: Socialbakers Listening API
  slug: socialbakers-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-listening-api-openapi.yml
- filename: socialbakers-posts-api-openapi.yml
  format: yaml
  label: Socialbakers Posts API
  slug: socialbakers-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-posts-api-openapi.yml
- filename: socialbakers-profile-metrics-api-openapi.yml
  format: yaml
  label: Socialbakers Profile Metrics API
  slug: socialbakers-profile-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-profile-metrics-api-openapi.yml
- filename: socialbakers-reference-api-openapi.yml
  format: yaml
  label: Socialbakers Reference API
  slug: socialbakers-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-reference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emplifi.io
  spf: true
hosts:
- cert_expires: Nov  5 11:37:58 2026 GMT
  host: api.emplifi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socialbakers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socialbakers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Socialbakers
provider_slug: socialbakers
slug: socialbakers-domain-security
source_filename: socialbakers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.emplifi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 11:37:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emplifi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/security/socialbakers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Social-Media
- Analytics
- Social Media Analytics
- Social Listening
- Marketing Analytics
- Digital Asset Management
- Customer Care
- Emplifi
---
