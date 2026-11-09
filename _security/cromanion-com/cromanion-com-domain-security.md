---
api_specs:
- filename: cromanion-com-openapi-generated.yml
  format: yaml
  label: Cromanion API
  slug: cromanion-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cromanion-com/openapi/_ae-authored/cromanion-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cromanion.com
  spf: true
hosts:
- cert_expires: Dec 16 13:01:50 2026 GMT
  host: cromanion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cromanion Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cromanion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cromanion
provider_slug: cromanion-com
slug: cromanion-com-domain-security
source_filename: cromanion-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cromanion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 13:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cromanion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cromanion-com/security/cromanion-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- CRO
- Conversion
- Marketing
- Software-as-a-Service
---
