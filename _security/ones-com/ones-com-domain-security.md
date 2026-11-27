---
api_specs:
- filename: ones-com-openapi-generated.yml
  format: yaml
  label: ONES.com API
  slug: ones-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ones-com/openapi/_ae-authored/ones-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ones.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: ones.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ONES.com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ONES.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ONES.com
provider_slug: ones-com
slug: ones-com-domain-security
source_filename: ones-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: ones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ones-com/security/ones-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Project Management
- Knowledge Management
- Enterprise
---
