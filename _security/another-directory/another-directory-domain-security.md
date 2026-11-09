---
api_specs:
- filename: another-directory-categories-api-openapi.yml
  format: yaml
  label: Another Directory Categories API
  slug: another-directory-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/another-directory/openapi/another-directory-categories-api-openapi.yml
- filename: another-directory-submissions-api-openapi.yml
  format: yaml
  label: Another Directory Submissions API
  slug: another-directory-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/another-directory/openapi/another-directory-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: another.directory
  spf: true
hosts:
- cert_expires: Jan  6 19:58:20 2027 GMT
  host: another.directory
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Another Directory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Another Directory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Another Directory
provider_slug: another-directory
slug: another-directory-domain-security
source_filename: another-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: another.directory\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 19:58:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: another.directory\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/another-directory/security/another-directory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
