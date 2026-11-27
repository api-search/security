---
api_specs:
- filename: labii-openapi-generated.yml
  format: yaml
  label: Labii API
  slug: labii-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/labii/openapi/_ae-authored/labii-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: labii.com
  spf: true
hosts:
- cert_expires: May  7 23:59:59 2027 GMT
  host: www.labii.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Labii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labii, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Labii
provider_slug: labii
slug: labii-domain-security
source_filename: labii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.labii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: labii.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/labii/security/labii-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- ELN
- LIMS
- Laboratory
- Digital Health
- Software-as-a-Service
---
