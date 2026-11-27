---
api_specs:
- filename: getcims-com-creators-api-openapi.yml
  format: yaml
  label: CIMS Creators API
  slug: getcims-com-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcims-com/openapi/getcims-com-creators-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getcims.com
  spf: true
hosts:
- cert_expires: Jan 12 13:36:01 2027 GMT
  host: getcims.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CIMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CIMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CIMS
provider_slug: getcims-com
slug: getcims-com-domain-security
source_filename: getcims-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcims.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:36:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getcims.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getcims-com/security/getcims-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Influencer Marketing
- Software-as-a-Service
- Campaign Management
- Analytics
- Marketing
---
