---
api_specs:
- filename: databutler-dev-openapi-generated.yml
  format: yaml
  label: databutler-dev API
  slug: databutler-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databutler-dev/openapi/_ae-authored/databutler-dev-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: databutler.dev
  spf: false
hosts:
- cert_expires: Jan  7 22:27:21 2027 GMT
  host: databutler.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Databutler Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for databutler-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: databutler-dev
provider_slug: databutler-dev
slug: databutler-dev-domain-security
source_filename: databutler-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: databutler.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:27:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: databutler.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/databutler-dev/security/databutler-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data
- API
- Tax
- Reference
---
