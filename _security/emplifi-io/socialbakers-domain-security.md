---
api_specs:
- filename: emplifi-io-ads-api-openapi.yml
  format: yaml
  label: Emplifi Ads API
  slug: emplifi-io-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-ads-api-openapi.yml
- filename: emplifi-io-assets-api-openapi.yml
  format: yaml
  label: Emplifi Assets API
  slug: emplifi-io-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-assets-api-openapi.yml
- filename: emplifi-io-care-api-openapi.yml
  format: yaml
  label: Emplifi Care API
  slug: emplifi-io-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-care-api-openapi.yml
- filename: emplifi-io-community-api-openapi.yml
  format: yaml
  label: Emplifi Community API
  slug: emplifi-io-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-community-api-openapi.yml
- filename: emplifi-io-listening-api-openapi.yml
  format: yaml
  label: Emplifi Listening API
  slug: emplifi-io-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-listening-api-openapi.yml
- filename: emplifi-io-posts-api-openapi.yml
  format: yaml
  label: Emplifi Posts API
  slug: emplifi-io-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-posts-api-openapi.yml
- filename: emplifi-io-profile-metrics-api-openapi.yml
  format: yaml
  label: Emplifi Profile Metrics API
  slug: emplifi-io-profile-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-profile-metrics-api-openapi.yml
- filename: emplifi-io-reference-api-openapi.yml
  format: yaml
  label: Emplifi Reference API
  slug: emplifi-io-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-reference-api-openapi.yml
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
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Socialbakers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emplifi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Emplifi
provider_slug: emplifi-io
slug: socialbakers-domain-security
source_filename: socialbakers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.emplifi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 11:37:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emplifi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/security/socialbakers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Social Media
- Analytics
- Social Media Analytics
- Social Listening
- Marketing Analytics
- Digital Asset Management
- Customer Care
- Emplifi
---
