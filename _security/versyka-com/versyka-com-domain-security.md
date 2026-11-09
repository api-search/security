---
api_specs:
- filename: versyka-com-openapi-generated.yml
  format: yaml
  label: versyka-com API
  slug: versyka-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/versyka-com/openapi/_ae-authored/versyka-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: versyka.com
  spf: true
hosts:
- cert_expires: Jan  6 22:09:13 2027 GMT
  host: versyka.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Versyka Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for versyka-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: versyka-com
provider_slug: versyka-com
slug: versyka-com-domain-security
source_filename: versyka-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: versyka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 22:09:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: versyka.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/versyka-com/security/versyka-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Monitoring
- Developer Tools
- Automation
- Change Management
- Open Source
---
