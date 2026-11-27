---
api_specs:
- filename: commoninja-com-openapi-generated.yml
  format: yaml
  label: Common Ninja Platform API
  slug: commoninja-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commoninja-com/openapi/_ae-authored/commoninja-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commoninja.com
  spf: true
hosts:
- cert_expires: Jan 13 09:57:39 2027 GMT
  host: www.commoninja.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Common Ninja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common Ninja, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Common Ninja
provider_slug: commoninja-com
slug: commoninja-com-domain-security
source_filename: commoninja-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commoninja.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 09:57:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commoninja.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/commoninja-com/security/commoninja-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Widgets
- No-Code
- Website Builder
- White Label
- Webhook
- E-Commerce
- Developer Platform
---
