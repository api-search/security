---
api_specs:
- filename: harvv-com-openapi-generated.yml
  format: yaml
  label: Harvv API
  slug: harvv-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvv-com/openapi/_ae-authored/harvv-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: harvv.com
  spf: true
hosts:
- cert_expires: May 12 23:59:59 2027 GMT
  host: harvv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Harvv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harvv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Harvv
provider_slug: harvv-com
slug: harvv-com-domain-security
source_filename: harvv-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harvv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: harvv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/harvv-com/security/harvv-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Behavioral Analytics
- Website Analytics
- Session Analysis
- dead‑click detection
---
