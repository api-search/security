---
api_specs:
- filename: notipo-com-openapi-generated.yml
  format: yaml
  label: Notipo API
  slug: notipo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notipo-com/openapi/_ae-authored/notipo-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notipo.com
  spf: true
hosts:
- cert_expires: Jan 14 16:36:36 2027 GMT
  host: notipo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Notipo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notipo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Notipo
provider_slug: notipo-com
slug: notipo-com-domain-security
source_filename: notipo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notipo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 16:36:36 2027 GMT\n  hsts: false\ndomains:\n- domain: notipo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/notipo-com/security/notipo-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- WordPress
- Publishing
- Automation
- Integration
---
