---
api_specs:
- filename: datadoe-com-openapi-generated.yml
  format: yaml
  label: DataDoe API
  slug: datadoe-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datadoe-com/openapi/_ae-authored/datadoe-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datadoe.com
  spf: true
hosts:
- cert_expires: May  4 23:59:59 2027 GMT
  host: datadoe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datadoe Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataDoe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DataDoe
provider_slug: datadoe-com
slug: datadoe-com-domain-security
source_filename: datadoe-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datadoe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datadoe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datadoe-com/security/datadoe-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DataDoe
- Amazon
- Artificial Intelligence
- MCP
- DataLayer
- Software-as-a-Service
---
