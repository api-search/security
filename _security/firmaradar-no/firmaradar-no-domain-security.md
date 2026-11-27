---
api_specs:
- filename: firmaradar-no-openapi-generated.yml
  format: yaml
  label: Firmaradar API
  slug: firmaradar-no-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmaradar-no/openapi/_ae-authored/firmaradar-no-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firmaradar.no
  spf: true
hosts:
- cert_expires: Dec 23 23:33:46 2026 GMT
  host: firmaradar.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmaradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firmaradar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Firmaradar
provider_slug: firmaradar-no
slug: firmaradar-no-domain-security
source_filename: firmaradar-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firmaradar.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firmaradar.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/firmaradar-no/security/firmaradar-no-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- KYC
- AML
- Credit
---
