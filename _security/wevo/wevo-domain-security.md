---
api_specs:
- filename: wevo-wevo-api-api-openapi.yml
  format: yaml
  label: Wevo API
  slug: wevo-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wevo/openapi/wevo-wevo-api-api-openapi.yml
- filename: wevo-openapi-generated.yml
  format: yaml
  label: Wevo API
  slug: wevo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wevo/openapi/_ae-authored/wevo-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wevo.com.br
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: wevo.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wevo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wevo
provider_slug: wevo
slug: wevo-domain-security
source_filename: wevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wevo.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wevo.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wevo/security/wevo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Integration
- Automation
- iPaaS
- API Management
- Low-code
- Artificial Intelligence
- EDI
---
