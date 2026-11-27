---
api_specs:
- filename: neverapply-co-expiredjobs-api-openapi.yml
  format: yaml
  label: NeverApply Expired Jobs API
  slug: neverapply-co-expiredjobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-expiredjobs-api-openapi.yml
- filename: neverapply-co-feed-api-openapi.yml
  format: yaml
  label: NeverApply Feed API
  slug: neverapply-co-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-feed-api-openapi.yml
- filename: neverapply-co-jobs-api-openapi.yml
  format: yaml
  label: NeverApply Jobs API
  slug: neverapply-co-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-jobs-api-openapi.yml
- filename: neverapply-co-meta-api-openapi.yml
  format: yaml
  label: NeverApply Meta API
  slug: neverapply-co-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-meta-api-openapi.yml
- filename: neverapply-co-search-api-openapi.yml
  format: yaml
  label: NeverApply Search API
  slug: neverapply-co-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: neverapply.co
  spf: true
hosts:
- cert_expires: Feb 11 18:04:31 2027 GMT
  host: neverapply.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NeverApply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeverApply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NeverApply
provider_slug: neverapply-co
slug: neverapply-co-domain-security
source_filename: neverapply-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neverapply.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 18:04:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neverapply.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/neverapply-co/security/neverapply-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Job Search
- Automation
- Recruiting
- Software-as-a-Service
---
