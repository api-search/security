---
api_specs:
- filename: peoplehr-openapi-generated.yml
  format: yaml
  label: PeopleHR API
  slug: peoplehr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peoplehr/openapi/_ae-authored/peoplehr-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peoplehr.com
  spf: true
hosts:
- cert_expires: Dec  1 04:54:57 2026 GMT
  host: www.peoplehr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Peoplehr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PeopleHR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PeopleHR
provider_slug: peoplehr
slug: peoplehr-domain-security
source_filename: peoplehr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peoplehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 04:54:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peoplehr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/peoplehr/security/peoplehr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HR
- SaaS
- Payroll
- Recruitment
- HRTech
- EmployeeManagement
---
