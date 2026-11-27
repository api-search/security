---
api_specs:
- filename: logospell-com-openapi-generated.yml
  format: yaml
  label: Logospell API
  slug: logospell-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logospell-com/openapi/_ae-authored/logospell-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logospell.com
  spf: true
hosts:
- cert_expires: Jan 24 22:54:31 2027 GMT
  host: logospell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Logospell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logospell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Logospell
provider_slug: logospell-com
slug: logospell-com-domain-security
source_filename: logospell-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logospell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 22:54:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: logospell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/logospell-com/security/logospell-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Image Generation
- MCP
- Software-as-a-Service
- Creative Tools
---
