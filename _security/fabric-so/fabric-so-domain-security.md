---
api_specs:
- filename: fabric-so-openapi-generated.yml
  format: yaml
  label: Fabric API
  slug: fabric-so-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabric-so/openapi/_ae-authored/fabric-so-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fabric.so
  spf: true
hosts:
- cert_expires: Jan 13 19:49:02 2027 GMT
  host: fabric.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fabric So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fabric
provider_slug: fabric-so
slug: fabric-so-domain-security
source_filename: fabric-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabric.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 19:49:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fabric.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fabric-so/security/fabric-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Workspace
- File Storage
- Integrations
---
