---
api_specs:
- filename: asoatlas-com-openapi-generated.yml
  format: yaml
  label: ASO Atlas API
  slug: asoatlas-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoatlas-com/openapi/_ae-authored/asoatlas-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asoatlas.com
  spf: true
hosts:
- cert_expires: Jan 12 23:18:10 2027 GMT
  host: asoatlas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asoatlas Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASO Atlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ASO Atlas
provider_slug: asoatlas-com
slug: asoatlas-com-domain-security
source_filename: asoatlas-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asoatlas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:18:10 2027 GMT\n  hsts: false\ndomains:\n- domain: asoatlas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/asoatlas-com/security/asoatlas-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ASO
- App Store
- Keyword Research
- Analytics
- Software-as-a-Service
---
