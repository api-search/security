---
api_specs:
- filename: citizenleap-com-openapi-generated.yml
  format: yaml
  label: Civica API
  slug: citizenleap-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citizenleap-com/openapi/_ae-authored/citizenleap-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: citizenleap.com
  spf: true
hosts:
- cert_expires: Jan 12 17:49:43 2027 GMT
  host: citizenleap.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Civica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Civica
provider_slug: citizenleap-com
slug: citizenleap-com-domain-security
source_filename: citizenleap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citizenleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:49:43 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: citizenleap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/citizenleap-com/security/citizenleap-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Citizenship
- Test Prep
- Software-as-a-Service
- Civica
---
