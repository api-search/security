---
api_specs:
- filename: sourcepost-interest-api-openapi.yml
  format: yaml
  label: SourcePost Interest API
  slug: sourcepost-interest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sourcepost/openapi/sourcepost-interest-api-openapi.yml
- filename: sourcepost-listings-api-openapi.yml
  format: yaml
  label: SourcePost Listings API
  slug: sourcepost-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sourcepost/openapi/sourcepost-listings-api-openapi.yml
- filename: sourcepost-system-api-openapi.yml
  format: yaml
  label: SourcePost System API
  slug: sourcepost-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sourcepost/openapi/sourcepost-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sourcepost.dev
  spf: true
hosts:
- cert_expires: Jan 29 13:54:11 2027 GMT
  host: sourcepost.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SourcePost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SourcePost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SourcePost
provider_slug: sourcepost
slug: sourcepost-domain-security
source_filename: sourcepost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourcepost.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 13:54:11 2027 GMT\n  hsts: null\ndomains:\n- domain: sourcepost.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sourcepost/security/sourcepost-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Directory
- Suppliers
- Data
- Agents
---
