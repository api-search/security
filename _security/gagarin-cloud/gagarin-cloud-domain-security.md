---
api_specs:
- filename: gagarin-cloud-openapi-generated.yml
  format: yaml
  label: Gagarin API
  slug: gagarin-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gagarin-cloud/openapi/_ae-authored/gagarin-cloud-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gagarin.cloud
  spf: false
hosts:
- cert_expires: Feb  1 14:40:44 2027 GMT
  host: gagarin.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gagarin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gagarin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Gagarin
provider_slug: gagarin-cloud
slug: gagarin-cloud-domain-security
source_filename: gagarin-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gagarin.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 14:40:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gagarin.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gagarin-cloud/security/gagarin-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Deployment
- Monitoring
- Alerts
- Logging
- Company
---
