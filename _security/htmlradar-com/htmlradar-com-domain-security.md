---
api_specs:
- filename: htmlradar-com-openapi-generated.yml
  format: yaml
  label: HTMLRadar API
  slug: htmlradar-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/htmlradar-com/openapi/_ae-authored/htmlradar-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: htmlradar.com
  spf: true
hosts:
- cert_expires: Feb  5 08:38:44 2027 GMT
  host: htmlradar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HTMLRadar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTMLRadar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HTMLRadar
provider_slug: htmlradar-com
slug: htmlradar-com-domain-security
source_filename: htmlradar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: htmlradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 08:38:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: htmlradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/htmlradar-com/security/htmlradar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tracking
- Analytics
- Document Sharing
- Software-as-a-Service
---
