---
api_specs:
- filename: crustdata-com-openapi-generated.yml
  format: yaml
  label: Crustdata API
  slug: crustdata-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crustdata-com/openapi/_ae-authored/crustdata-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crustdata.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: crustdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crustdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crustdata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crustdata
provider_slug: crustdata-com
slug: crustdata-com-domain-security
source_filename: crustdata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crustdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crustdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crustdata-com/security/crustdata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Data
- Artificial Intelligence
- Real-Time
- Company
---
