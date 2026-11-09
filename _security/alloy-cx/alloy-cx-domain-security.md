---
api_specs:
- filename: alloy-cx-openapi-generated.yml
  format: yaml
  label: Alloy API
  slug: alloy-cx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-cx/openapi/_ae-authored/alloy-cx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alloy.cx
  spf: true
hosts:
- cert_expires: Dec 23 18:47:56 2026 GMT
  host: alloy.cx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alloy Cx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alloy
provider_slug: alloy-cx
slug: alloy-cx-domain-security
source_filename: alloy-cx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alloy.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:47:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alloy.cx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/alloy-cx/security/alloy-cx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Artificial Intelligence
- Investment
- Automation
- CRM
---
