---
api_specs:
- filename: data247-com-openapi-generated.yml
  format: yaml
  label: Data247 API
  slug: data247-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/data247-com/openapi/_ae-authored/data247-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: data247.com
  spf: true
hosts:
- cert_expires: Jan 11 00:58:14 2027 GMT
  host: data247.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Data247 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data247, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Data247
provider_slug: data247-com
slug: data247-com-domain-security
source_filename: data247-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data247.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 00:58:14 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: data247.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/data247-com/security/data247-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Management
- Data Enrichment
- Validation
- Integration
---
