---
api_specs:
- filename: juzpost-accounts-api-openapi.yml
  format: yaml
  label: JuzPost Accounts API
  slug: juzpost-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-accounts-api-openapi.yml
- filename: juzpost-identity-api-openapi.yml
  format: yaml
  label: JuzPost Identity API
  slug: juzpost-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-identity-api-openapi.yml
- filename: juzpost-posts-api-openapi.yml
  format: yaml
  label: JuzPost Posts API
  slug: juzpost-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-posts-api-openapi.yml
- filename: juzpost-scheduling-api-openapi.yml
  format: yaml
  label: JuzPost Scheduling API
  slug: juzpost-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-scheduling-api-openapi.yml
- filename: juzpost-storage-api-openapi.yml
  format: yaml
  label: JuzPost Storage API
  slug: juzpost-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-storage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: juzpost.com
  spf: true
hosts:
- cert_expires: Jan  4 03:49:42 2027 GMT
  host: www.juzpost.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JuzPost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JuzPost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JuzPost
provider_slug: juzpost
slug: juzpost-domain-security
source_filename: juzpost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.juzpost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 03:49:42 2027 GMT\n  hsts: false\ndomains:\n- domain: juzpost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/juzpost/security/juzpost-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media
- Scheduling
- Automation
- Artificial Intelligence
- Marketing
---
