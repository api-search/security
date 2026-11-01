---
api_specs:
- filename: chorus-pro-openapi-generated.yml
  format: yaml
  label: Chorus Pro API
  slug: chorus-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chorus-pro/openapi/_ae-authored/chorus-pro-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gouv.fr
  spf: true
hosts:
- cert_expires: Jan  7 12:14:00 2027 GMT
  host: chorus-pro.gouv.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chorus Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chorus Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chorus Pro
provider_slug: chorus-pro
slug: chorus-pro-domain-security
source_filename: chorus-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chorus-pro.gouv.fr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 12:14:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gouv.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chorus-pro/security/chorus-pro-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Payments
- PublicSector
- France
- E-invoicing
---
