---
api_specs:
- filename: citestamp-com-openapi-generated.yml
  format: yaml
  label: CiteStamp API
  slug: citestamp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citestamp-com/openapi/_ae-authored/citestamp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citestamp.com
  spf: true
hosts:
- cert_expires: Jan  4 18:29:16 2027 GMT
  host: citestamp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 05:13:57 2027 GMT
  host: api.citestamp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: CiteStamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CiteStamp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CiteStamp
provider_slug: citestamp-com
slug: citestamp-com-domain-security
source_filename: citestamp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citestamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 18:29:16 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.citestamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 05:13:57 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: citestamp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/citestamp-com/security/citestamp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Citation Graph
- Scholarly Metadata
- Bibliography Checking
- AI Integration
- Publishers
---
