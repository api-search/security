---
api_specs:
- filename: socialdata-tools-data-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Data API
  slug: socialdata-tools-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-data-api-api-openapi.yml
- filename: socialdata-tools-monitoring-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Monitoring API
  slug: socialdata-tools-monitoring-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-monitoring-api-api-openapi.yml
- filename: socialdata-tools-social-actions-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Social Actions API
  slug: socialdata-tools-social-actions-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-social-actions-api-api-openapi.yml
- filename: socialdata-tools-socialdata-account-management-api-openapi.yml
  format: yaml
  label: socialdata-tools SocialData Account Management API
  slug: socialdata-tools-socialdata-account-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-socialdata-account-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: socialdata.tools
  spf: true
hosts:
- cert_expires: Jan 11 07:56:17 2027 GMT
  host: socialdata.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Socialdata Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for socialdata-tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: socialdata-tools
provider_slug: socialdata-tools
slug: socialdata-tools-domain-security
source_filename: socialdata-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socialdata.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 07:56:17 2027 GMT\n  hsts: false\ndomains:\n- domain: socialdata.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/socialdata-tools/security/socialdata-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API
- Data
- Social Media
- X
- Twitter
---
