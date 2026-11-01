---
api_specs:
- filename: withvector-com-openapi-generated.yml
  format: yaml
  label: Vector API
  slug: withvector-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withvector-com/openapi/_ae-authored/withvector-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: withvector.com
  spf: true
hosts:
- cert_expires: Jan 12 22:34:09 2027 GMT
  host: withvector.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Withvector Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vector, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vector
provider_slug: withvector-com
slug: withvector-com-domain-security
source_filename: withvector-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withvector.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 22:34:09 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: withvector.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/withvector-com/security/withvector-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- APIs
- Platform
- Enterprise
---
