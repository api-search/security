---
api_specs:
- filename: accoil-accoil-api-api-openapi.yml
  format: yaml
  label: Accoil API
  slug: accoil-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accoil/openapi/accoil-accoil-api-api-openapi.yml
- filename: accoil-openapi-generated.yml
  format: yaml
  label: Accoil API
  slug: accoil-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accoil/openapi/_ae-authored/accoil-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accoil.com
  spf: true
hosts:
- cert_expires: Jan 15 06:54:02 2027 GMT
  host: www.accoil.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accoil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accoil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Accoil
provider_slug: accoil
slug: accoil-domain-security
source_filename: accoil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accoil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 06:54:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: accoil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/accoil/security/accoil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retention
- Expansion
- Customer Success
- Playbook
- Analytics
---
