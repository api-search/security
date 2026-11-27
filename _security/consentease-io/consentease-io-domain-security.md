---
api_specs:
- filename: consentease-io-openapi-generated.yml
  format: yaml
  label: ConsentEase API
  slug: consentease-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consentease-io/openapi/_ae-authored/consentease-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: consentease.io
  spf: false
hosts:
- cert_expires: Jan 26 23:45:14 2027 GMT
  host: consentease.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ConsentEase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConsentEase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ConsentEase
provider_slug: consentease-io
slug: consentease-io-domain-security
source_filename: consentease-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: consentease.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:45:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: consentease.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/consentease-io/security/consentease-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GDPR
- CCPA
- Cookie Consent
- Small Business
---
