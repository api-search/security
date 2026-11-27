---
api_specs:
- filename: harvis-dev-files-api-openapi.yml
  format: yaml
  label: Harvis Files API
  slug: harvis-dev-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-files-api-openapi.yml
- filename: harvis-dev-keys-api-openapi.yml
  format: yaml
  label: Harvis Keys API
  slug: harvis-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-keys-api-openapi.yml
- filename: harvis-dev-meta-api-openapi.yml
  format: yaml
  label: Harvis Meta API
  slug: harvis-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-meta-api-openapi.yml
- filename: harvis-dev-sites-api-openapi.yml
  format: yaml
  label: Harvis Sites API
  slug: harvis-dev-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-sites-api-openapi.yml
- filename: harvis-dev-submissions-api-openapi.yml
  format: yaml
  label: Harvis Submissions API
  slug: harvis-dev-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: harvis.dev
  spf: true
hosts:
- cert_expires: Jan 17 23:26:04 2027 GMT
  host: harvis.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Harvis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harvis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Harvis
provider_slug: harvis-dev
slug: harvis-dev-domain-security
source_filename: harvis-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harvis.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:26:04 2027 GMT\n  hsts: false\ndomains:\n- domain: harvis.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/harvis-dev/security/harvis-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deployment
- Static Sites
- Developer Tools
---
