---
api_specs:
- filename: statespace-gg-openapi-generated.yml
  format: yaml
  label: Statespace API
  slug: statespace-gg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/statespace-gg/openapi/_ae-authored/statespace-gg-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: statespace.com
  spf: true
hosts:
- cert_expires: Jan 20 03:48:06 2027 GMT
  host: statespace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statespace Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statespace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Statespace
provider_slug: statespace-gg
slug: statespace-gg-domain-security
source_filename: statespace-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statespace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 03:48:06 2027 GMT\n  hsts: false\ndomains:\n- domain: statespace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/statespace-gg/security/statespace-gg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Simulation
- Analytics
- Cloud
- Engineering
---
