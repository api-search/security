---
api_specs:
- filename: homebox-software-openapi-generated.yml
  format: yaml
  label: HomeBox API
  slug: homebox-software-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homebox-software/openapi/_ae-authored/homebox-software-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: homebox.software
  spf: true
hosts:
- cert_expires: Jan 12 13:31:20 2027 GMT
  host: homebox.software
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Homebox Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeBox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HomeBox
provider_slug: homebox-software
slug: homebox-software-domain-security
source_filename: homebox-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homebox.software\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:31:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: homebox.software\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/homebox-software/security/homebox-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Home
- Inventory
- OpenSource
- SelfHosted
- Go
---
