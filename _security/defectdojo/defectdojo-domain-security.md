---
api_specs:
- filename: defectdojo-openapi-generated.yml
  format: yaml
  label: DefectDojo API
  slug: defectdojo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defectdojo/openapi/_ae-authored/defectdojo-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: defectdojo.com
  spf: true
hosts:
- cert_expires: Feb  3 20:27:19 2027 GMT
  host: defectdojo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DefectDojo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DefectDojo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DefectDojo
provider_slug: defectdojo
slug: defectdojo-domain-security
source_filename: defectdojo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defectdojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 20:27:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: defectdojo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/defectdojo/security/defectdojo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vulnerability Management
- Application Security
- DevSecOps
- Compliance
- Penetration Testing
- SOC
- psirt
- Cloud Security
---
