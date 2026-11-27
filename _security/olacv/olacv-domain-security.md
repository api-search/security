---
api_specs:
- filename: olacv-openapi-generated.yml
  format: yaml
  label: Ola CV API
  slug: olacv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/olacv/openapi/_ae-authored/olacv-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ola.cv
  spf: true
hosts:
- cert_expires: Jan 13 23:07:57 2027 GMT
  host: ola.cv
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ola CV Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ola CV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ola CV
provider_slug: olacv
slug: olacv-domain-security
source_filename: olacv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ola.cv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:07:57 2027 GMT\n  hsts: false\ndomains:\n- domain: ola.cv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/olacv/security/olacv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Domain Registry
- Marketplace
- Premium Domains
- API Integration
- Registrar Partnership
- Professional Branding
---
