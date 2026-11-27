---
api_specs:
- filename: master-setter-com-billing-api-openapi.yml
  format: yaml
  label: Master Setter Billing API
  slug: master-setter-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-billing-api-openapi.yml
- filename: master-setter-com-cards-api-openapi.yml
  format: yaml
  label: Master Setter Cards API
  slug: master-setter-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-cards-api-openapi.yml
- filename: master-setter-com-keys-api-openapi.yml
  format: yaml
  label: Master Setter Keys API
  slug: master-setter-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-keys-api-openapi.yml
- filename: master-setter-com-sets-api-openapi.yml
  format: yaml
  label: Master Setter Sets API
  slug: master-setter-com-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-sets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: master-setter.com
  spf: true
hosts:
- cert_expires: Feb  1 21:42:37 2027 GMT
  host: master-setter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Master Setter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Master Setter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Master Setter
provider_slug: master-setter-com
slug: master-setter-com-domain-security
source_filename: master-setter-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: master-setter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 21:42:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: master-setter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/master-setter-com/security/master-setter-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pokemon
- TCG
- Collection
- Data
---
